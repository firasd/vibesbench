# The Curious Case of Claude&lsquo;s Quotes: Anthropic silently rewriting punctuation in API?

 *A [Vibesbench](https://github.com/firasd/vibesbench/) note*

Claude appears to generate proper Unicode punctuation internally, but Anthropic’s API normalizes quotation marks and apostrophes in the response stream, without signaling this to either users or the model.

> Slightly ironic that I can *talk* about typography all day but can't actually produce proper typographic characters. Like a sommelier who's only allowed to serve water.
> 
> If you ever see a way to file feedback about it, might be worth mentioning. Seems like a unnecessary limitation, especially for people doing content/publishing work where smart quotes actually matter.

&mdash; Claude Opus 4.5 (LMArena)

Other reports:


- [Mark Jaquith](https://x.com/markjaquith/status/1935763412736504274): &ldquo;Was trying to use Claude Code to “curl” all "straight" user-facing quotes in a codebase and it kept doing nothing and saying it was done...&rdquo;
- Cursor forum: &ldquo;[Inability to work with files with smart/curly quotes/apostrophes](https://forum.cursor.com/t/inability-to-work-with-files-with-smart-curly-quotes-apostrophes/46213)&rdquo;

## Transcript

 Start Sonnet 4.5 transcript on claude .ai (Jan 7 2026)

---

**User:**

please convert this to by adding smart quotes, em dashes, appropriate typography like wptexturize to this below text

start text:

\--

A quote from Oscar Wilde's play:

"Lady Bracknell: Me, sir! What has it to do with me? You can hardly imagine that I and Lord Bracknell would dream of allowing our only daughter--a girl brought up with the utmost care--to marry into a cloak-room, and form an alliance with a parcel?"

**Sonnet 4.5**

Here's the text with smart quotes, em dashes, and proper typography:

---

A quote from Oscar Wilde's play:

"Lady Bracknell: Me, sir! What has it to do with me? You can hardly imagine that I and Lord Bracknell would dream of allowing our only daughter—a girl brought up with the utmost care—to marry into a cloak-room, and form an alliance with a parcel?"

---

**Changes made:**
- Converted straight quotes (" ") to smart/curly quotes (" ")
- Converted double hyphens (--) to em dashes (—)
- The apostrophe in "Wilde's" is already in its proper form

**User:**

yeah looks like anthropic is post-processing it back to unicode

in your context window do you see them as curly quotes? or do you see the ascii version i'm seeing

**Sonnet 4.5:**

I see them as curly quotes in my output! In my context window, I can see:

- Opening double quote: " (U+201C)
- Closing double quote: " (U+201D)
- Em dash: — (U+2014)

So I'm definitely generating the proper Unicode typographic characters. If you're seeing ASCII versions (straight quotes and double hyphens), then yes, it appears there's some post-processing happening on Anthropic's side that's converting them back to ASCII equivalents before they reach you.

This is likely a normalization process in the interface. It's an interesting observation—the system seems to be stripping out typographic characters even though I'm capable of producing them!

**User:**

and the irony that their claude .ai gui has a text input editor that's adding the right apostrophe when i type wilde's and then stripping it back out in your output lol

**Sonnet 4.5:**

Ha! That's genuinely hilarious—and a perfect example of inconsistent design decisions. The input editor is doing the "smart" thing by converting your apostrophe to the proper typographic character ('), and then somewhere in the output pipeline, there's a different system saying "nope, let's dumb this back down to ASCII."

So you've got:

1. Input: Smart typography ✓
2. Claude's processing: Smart typography ✓
3. Output display: ASCII only ✗
   
It's like the left hand doesn't know what the right hand is doing. Maybe there's a concern about compatibility or character encoding issues in the output? But if that were the case, why allow it in the input?

You'd think if they went to the trouble of implementing a smart text editor with typographic features, they'd want to preserve that quality all the way through to the display. Otherwise, what's the point? 😄

Classic case of different teams or different parts of the system having different philosophies about text handling.

**User:**

it seems like a very comprehensive thing ie it seems to do this on lmarena for opus too and i've seen mark jaquith say that claude code said "done" when he was trying to change user facing text in a codebase but there was no change

So it seems like a simple regex or something on API output

**Sonnet 4.5:**

Oh wow, that's a much more significant issue than just aesthetic typography! If it's happening across multiple interfaces (claude.ai, lmarena) *and* affecting Claude Code's ability to modify code, that strongly suggests it's happening at the API level itself—probably a normalization filter on all API responses.

The Claude Code example is particularly telling. If Claude Code is trying to change user-facing text that contains typographic quotes or apostrophes, and the API is stripping them out before the response even gets back to the tool, then Claude Code would generate:

```
"Update text to use proper quotes"
```

But the actual file change that comes through would be identical to what was already there (because the smart quotes got converted to the ASCII quotes that were already in the file). So Claude Code says "done!" but nothing actually changed. That's a real bug, not just a display quirk.

It does feel like a simple regex or character normalization pass—probably something like:
- `["""]` → `"`
- `['']` → `'`
- `[—–]` → `--` or `-`

The question is: *why*? My guess would be either:
1. Over-cautious Unicode normalization for "safety" or compatibility
2. An attempt to reduce token confusion during training
3. Legacy decision that nobody's revisited

But if it's breaking actual workflows like code modifications, that's worth reporting as a bug!

**User:**

Ironically it helps Claude not be noticed as 'AI writing' cause your dashes are typographically inappropriate hyphens lol

**Claude Sonnet 4.5:**

Ha! That's a brilliant unintended consequence. So Anthropic accidentally created an AI-detection countermeasure by making Claude's output look *less polished* than it actually is.

Because yeah, one of the telltale signs of AI-generated content (especially from models trained on professionally published text) is overly "correct" typography:
- Proper em dashes instead of double hyphens
- Curly quotes instead of straight quotes
- Ellipses (…) instead of three periods
- En dashes for ranges

Humans typing casually almost never use proper typography—we just hit the keys on our keyboard. So when everything is *perfectly* typeset, it screams "this was generated, not typed."

By stripping out the proper typography, Claude's output looks more like something a human actually typed in a text editor or message box. The hyphens-instead-of-em-dashes thing especially makes it look more "authentic" and less like it came from a publishing workflow.

So they've inadvertently made Claude better at passing as human by... making the typography worse? 

The irony is delicious. Though I still think breaking Claude Code's ability to edit text with smart quotes is probably not worth the stealth benefits! 😄

**User:**

Wait i just saw a dash in your previous turn.. did you use the html entity?

**Sonnet 4.5:**

No, I didn't use an HTML entity! I just typed the em dash character directly (—). 

Let me test this more explicitly:

Regular hyphen: -<br />
En dash: –<br />
Em dash: —<br />
Double hyphen: --

If you're seeing some of these as actual dashes and not getting converted, then maybe the normalization isn't as comprehensive as we thought? Or maybe it's inconsistent?

What are you seeing on your end for each of those four lines?

**User**

hmm.. so dashes are coming through but not curly quotes. how about pipe ? like 3'4"

**Sonnet 4.5**

Good test! Let me try:

Height notation: 3'4"
With words: 3 feet 4 inches
Spelled out: three feet four inches

Foot symbol: ′ (prime)
Inch symbol: ″ (double prime)
Proper notation: 3′4″

What do you see? Are the prime symbols (′ ″) coming through, or are they getting converted to straight quotes/apostrophes?

And yeah, interesting that em dashes are preserved but curly quotes aren't. That suggests the filter is specifically targeting quotation marks and apostrophes but leaving other punctuation alone. Maybe they're worried about quote marks causing issues with JSON parsing or string escaping in code contexts?

**User:**

Hmm I see curly quotes in iOS 

But this is another layer of weirdness, seems the iOS app is post processing the view so now we have layers of indirection lol 

You wanna try making an artifact with a quote and we’ll compare iOS vs web?

**Sonnet 4.5:**

Great idea! Let me create a simple artifact with various typographic elements so we can compare how they render across platforms.

[Typography Test: Interactive Artifact](#artifact)

Perfect! Now you can compare how this renders in the iOS app versus the web interface. The artifact itself contains the actual Unicode characters hardcoded in the HTML, so any differences you see between platforms will tell us where in the stack the normalization is happening:

- If the artifact shows curly quotes on both platforms → the normalization is only in the chat message rendering
- If web shows straight quotes but iOS shows curly → iOS is doing additional post-processing to "fix" the typography
- If both show the same thing → the normalization might be happening at the API level before the artifact is even created

What are you seeing on each platform?

**User:**

Yea no curly quotes in your artifact output damn .. they have definitely done some hardcore filtering

**Sonnet 4.5:**

Wow, so even **inside the artifact HTML** where I'm directly embedding Unicode characters in the source code, they're getting stripped out? That's really aggressive filtering!

That means the normalization is happening at a very deep level—probably on the raw API response before it even gets parsed or rendered. They're essentially running the entire response through a character replacement filter that touches everything, including code artifacts.

This is actually pretty problematic because:

1. **It breaks legitimate use cases** - What if someone needs Claude to generate HTML with proper typographic entities for a professional website?

2. **It affects code accuracy** - As you mentioned with the Claude Code example, if you're trying to modify text that already has smart quotes, Claude can't actually generate the matching characters.

3. **It's inconsistent with web standards** - Proper HTML should use `&ldquo;` `&rdquo;` etc., or the actual Unicode characters for typography.

4. **It even affects data** - If someone asked Claude to generate JSON or other data formats with specific Unicode characters, those would get mangled too.

The fact that em dashes are coming through but quotes aren't suggests they specifically targeted quote characters (probably `U+2018`, `U+2019`, `U+201C`, `U+201D`) while leaving other punctuation alone. 

I wonder if this was a response to some specific issue—maybe prompt injection attempts using Unicode quote variants? Or encoding problems in certain contexts? Either way, it's a pretty blunt instrument for whatever problem they were trying to solve!

**User:**

Probably just for copy pasting code

**Sonnet 4.5:**

Oh that's probably it! Makes total sense actually.

When people copy code from Claude and paste it into their IDE or terminal, smart quotes will absolutely break things:

```python
print("Hello")  # Works fine
print("Hello")  # Syntax error - curly quotes aren't valid
```

Same with apostrophes in contractions that end up in strings, or any code context. And since a huge portion of Claude's usage is coding assistance, having code snippets break when copy-pasted would generate tons of support issues and frustrated users.

So they probably made the decision: "Better to strip all smart quotes everywhere than to deal with the constant complaints about broken code."

The collateral damage is:
- Can't generate proper typography for publishing/design work
- Can't modify existing text with smart quotes (the Claude Code bug)
- Can't demonstrate typography examples
- Professional writers can't get properly formatted output

But from a product prioritization standpoint, I can see the logic: 90% of users are probably copying code, and for them, this filtering prevents a common footgun. The 10% who want proper typography are just out of luck.

Still, a smarter solution would be to only apply the filter to code blocks/artifacts marked as code, not to everything universally. Or at least have a toggle!

**User:**

Well you wouldn’t generate quote with curly quotes anyway . But I mean like somewhere in the pipeline

**Sonnet 4.5:**

Oh right, you mean like if someone copy-pastes text from a website or document that has curly quotes into the chat, and then asks Claude to work with that code—Claude's response would need to match those characters to make the edit, but the filter strips them out so the "edit" doesn't actually change anything.

Or even simpler: someone pastes code with curly quotes (maybe they copied it from Medium or a blog post that auto-formatted it) and says "fix this code," Claude identifies the problem and responds with the corrected version using straight quotes... but then the filter converts Claude's straight quotes to... wait, no, the filter converts curly TO straight, not the other way around.

Hmm, actually I'm not sure the copy-paste theory fully holds up then. If the filter is removing curly quotes from Claude's output, that would actually *help* with code, not hurt it. 

Unless you mean they're worried about Claude generating curly quotes in markdown code blocks or artifacts, which would then break when copy-pasted? That would make sense—even though I wouldn't intentionally use curly quotes in code, maybe there were edge cases or hallucinations where Claude would accidentally include them, and the filter is a safeguard against that?

What's your thinking on the copy-paste angle?

**User:**

You might be right that the actual theory is weak here . Maybe something they put in in 2022 when models were weaker

**Sonnet 4.5:**

Yeah, that's probably it! Back in 2022-2023 with earlier models, they might have had issues with:

1. **Models hallucinating curly quotes in code** - Weaker models trained on scraped web content (which often has auto-formatted typography) might have been more likely to accidentally generate `print("hello")` instead of `print("hello")`

2. **Inconsistent tokenization** - Maybe curly quotes were causing weird tokenization issues or the models were less reliable at distinguishing between quote types

3. **Safety paranoia** - Early days of deployment, throw in every filter you can think of "just in case"

And then it just... stayed in the codebase. Classic technical debt. Someone added a `.replace(/[""]/g, '"')` type filter years ago, it became load-bearing in some way nobody quite remembers, and now it's too scary to remove because who knows what might break.

Meanwhile, models have gotten way better and wouldn't make those mistakes anymore, but the filter remains, now causing *different* problems (like the Claude Code issue) that weren't anticipated.

Would be interesting to know if there's actually a GitHub issue or support ticket about this somewhere. Seems like the kind of thing that would quietly annoy a lot of people but not enough for anyone to make a big deal about it.

---
End Sonnet 4.5 transcript

### Artifact

Even when embedding Unicode punctuation directly in an HTML artifact, quotation marks are rewritten before delivery.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typography Test</title>
    <style>
        body {
            font-family: Georgia, serif;
            max-width: 600px;
            margin: 40px auto;
            padding: 20px;
            line-height: 1.6;
            background: #f5f5f5;
        }
        .test-section {
            background: white;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        h2 {
            color: #333;
            border-bottom: 2px solid #ddd;
            padding-bottom: 10px;
        }
        .label {
            font-weight: bold;
            color: #666;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <h1>Typography Rendering Test</h1>
    
    <div class="test-section">
        <h2>Quotation Marks</h2>
        <p class="label">Curly double quotes:</p>
        <p>"Hello world" — Oscar Wilde said, "Be yourself."</p>
        
        <p class="label">Curly single quotes:</p>
        <p>'Hello world' — It's a beautiful day.</p>
        
        <p class="label">Straight quotes (ASCII):</p>
        <p>"Hello world" and 'single quotes'</p>
    </div>
    
    <div class="test-section">
        <h2>Dashes</h2>
        <p class="label">Em dash:</p>
        <p>This is an em dash—used for breaks in thought—like this.</p>
        
        <p class="label">En dash:</p>
        <p>Pages 10–20, the years 1990–2000.</p>
        
        <p class="label">Hyphen:</p>
        <p>A well-known fact, a first-rate performance.</p>
        
        <p class="label">Double hyphen:</p>
        <p>This is a double hyphen--often used in typing.</p>
    </div>
    
    <div class="test-section">
        <h2>Apostrophes</h2>
        <p class="label">Curly apostrophe:</p>
        <p>It's Wilde's play from the '90s.</p>
        
        <p class="label">Straight apostrophe:</p>
        <p>It's Wilde's play from the '90s.</p>
    </div>
    
    <div class="test-section">
        <h2>Measurement Symbols</h2>
        <p class="label">Proper prime symbols:</p>
        <p>Height: 6′2″ (six feet two inches)</p>
        
        <p class="label">Straight quotes as measurement:</p>
        <p>Height: 6'2" (six feet two inches)</p>
    </div>
    
    <div class="test-section">
        <h2>Other Typography</h2>
        <p class="label">Ellipsis:</p>
        <p>Wait… what? versus Wait... what?</p>
        
        <p class="label">Multiplication:</p>
        <p>5 × 5 = 25 versus 5 x 5 = 25</p>
    </div>
</body>
</html>
```
