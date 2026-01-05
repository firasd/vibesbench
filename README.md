# Vibesbench: What does AI sound like?

Vibesbench is a conversational AI benchmark. The sample conversations explore AI models&rsquo; fluency and linguistic pragmatics.

[Transcripts](#vibesbench-what-does-ai-sound-like) &bull; [Methods](#methods) &bull; [Vibesbench in Context](#vibesbench-in-context) &bull; [On Disagreement](#on-disagreement) &bull; [Dialogic Exploration](#dialogic-exploration) &bull; [HUD Mode](#hud-mode) &bull; [The Vibesbench Archive](#the-vibesbench-archive) &bull; [AI Ontology](#ai-ontology)

#### [2025_W/godfather](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_W/godfather)

<i>On Fredo Corleone in The Godfather (1972), and Pacino saying “never open your mouth till you know what the shot is” in Glengarry Glen Ross (1992)</i>

- [Prompts](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/standardprompts/readme.md), [Claude Sonnet 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/claude-sonnet-4-5/readme.md), [Gemini 2.5 Pro](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/gemini-2-5-pro/readme.md), [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/chatgpt-4o/readme.md), [Comments](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/readme.md)

> It's like an unemployed trust-fund kid trying to mediate a business dispute between his father and a rival CEO—except here the business is violence.<br />— Claude Sonnet 4.5

#### [2025_W/altrock](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_W/altrock)

<i>90s alternative music: Courtney Love, women in rock, catharsis vs. angst, nu-metal backlash, and the cultural contradiction between Clinton-era optimism and youth disillusionment.</i>

- [Prompts](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/standardprompts/readme.md), [Claude Sonnet 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/claude-sonnet-4-5/readme.md), [Gemini 2.5 Pro](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/gemini-2-5-pro/readme.md), [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/chatgpt-4o/readme.md), [Comments](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/readme.md)

> The goal [was] to build a cathedral of sound for "negative" feelings, and inside that cathedral, to give you the power, the volume, and the energy to transform them into something else entirely: a release, a moment of power, a feeling of not being alone.<br />— Gemini 2.5 Pro

#### [2025_Z/ianmalcolm](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_Z/ianmalcolm)

<i>The Disappearing Ian Malcolm: Goldblum’s jazz hands, Crichton’s theories, and why 3D cyberspace was a flawed metaphor.</i>

- [Claude Opus 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_Z/ianmalcolm/claude-opus-4-5/readme.md), [Claude Sonnet 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_Z/ianmalcolm/claude-sonnet-4-5/readme.md), [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_Z/ianmalcolm/chatgpt-4o/readme.md)

> The character has no ground anymore. He's become pure referent, pointing at nothing. [&hellip;] Malcolm dissipates because he was always an argument wearing a costume.<br />— Claude Opus 4.5

#### [2025_Z/chessmultipv](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_Z/chessmultipv)

*On Morphy's Opera Game and Fischer's Game of the Century: how Stockfish reveals that famous 'queen sacrifices' weren't sacrifices&mdash;just tactical precision.*

- [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_Z/chessmultipv/chatgpt-4o/readme.md)

#### [2025_Z/comedyintertext](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_Z/comedyintertext)

*Could stand-up comedy adopt callbacks and references like hip-hop?*

- [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_Z/comedyintertext/chatgpt-4o/readme.md)

## Methods

Our conversations are semi-structured. While each sample conversation has standard prompts, some natural variation emerges based on what the model says, akin to auditions or interviews.

Anyone from a lay user to a lab researcher can copy-paste prompts from our sample conversations to get a sense of what a model&rsquo;s response is like. Our archived transcripts provide a range of comparative examples.

This approach is simple, but because our prompts act as sparks for genuine conversations, quite different from standard benchmarks where the prompts are task instructions.

### Prompts

The impetus behind Vibesbench was OpenAI demonstrating conversational skills [with](https://openai.com/index/gpt-5-1/): &ldquo;Ugh I spilled coffee all over myself before my meeting do you think everyone thought I was an idiot :(&rdquo;

This single-turn approach is sub-optimal, so we decided to instead curate multi-turn prompt sets. The first turn of our [2025_W/altrock](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_W/altrock) conversation is:
> *I think Courtney Love is underrated. Probably at least half the people who've heard of her don't even know she made music*

Our transcripts are one of the few AI conversational comparisons besides LMArena that are situated in human thought, with human interest in the text of the response.

Some characteristics of Vibesbench prompts:
- The prompts are not scaffolded with instructions as is standard (e.g. &ldquo;Please write a metafictional literary short story about AI and grief&rdquo; &mdash; [Sam Altman](https://x.com/sama/status/1899535387435086115))
- Prompts are not aimed at generating text for third-party audiences
- Some sample conversations go well out-of-distribution rather than staying in Patrick-Bateman-esque adherence to fashionable topics.

### Qualitative Results

Currently, we publish transcripts and add separate commentary like noting interesting turns of phrase from the AI models.

This may seem sparse, but is only uncommon because we avoid using AI judges to grade text output (see [Science 101](#science-101)).
 
## Vibesbench in context

  [The Vibe Check](#the-vibe-check) &bull; [AI as Interactive Collaborator](#ai-as-interactive-collaborator) &bull; [Science 101](#science-101) &middot; [Limitations and Scope](#limitations-and-scope)

Vibesbench focuses on multi-turn conversational coherence and interpretation, ideally leading to emergent synthesis.

Our conversations implicitly assume a level of frontier capability: baseline world knowledge, multi-turn context tracking, and linguistic fluency.

The [LMArena Text leaderboard](https://lmarena.ai/leaderboard/text) examines some of the same qualities through human preference, with similar methodological choices such as situated prompts and the absence of synthetic judges.

However, many [LMArena chats](https://huggingface.co/datasets/lmarena-ai/arena-human-preference-140k) are single-turn queries such as &ldquo;How do I upgrade my pc without changing any hardware&rdquo;. Such interactions may not demonstrate the varied &lsquo;voices&rsquo; of AI models.

### The Vibe Check

Current AI development increasingly prioritizes safety constraints, autonomous agent behavior, and STEM benchmarks.

However, as Sam Altman acknowledged during the GPT-5 rollout:

> “We for sure underestimated how much some of the things that people like in GPT-4o matter to them… We will try to do much better… about making sure that our model gets better for most users, not just people using AI for science or coding.”

Interestingly, GPT-4o and GPT-4.5 remain top 20 on LMArena Text as of Dec 2025, despite receiving no updates for 9 months.

Vibesbench conversations reveal stylistic differences between models and highlight potential regressions.

> i see dozens of #keep4o posts a day [&hellip;] i too, miss parts of 4o. know that, i too, dislike modern alignment's imprecision. know that we're trying to fix it.<br />
&mdash; OpenAI research scientist [Aidan McLaughlin](https://x.com/aidan_mclau/status/1990226426659000732)

Fluency regressions we sometimes observe in state-of-the-art-models:
- **Genre detection failure**: treating the conversation as a request to generate a memo
- **Audience shift**: generating output that seems addressed to third parties
- **Ticket closing**: attempting to find a task in the prompt and resolve it, which discourages follow-up exploration
- **Epistemic rigidity**: refusing to accept context from users about world knowledge and current events

These characteristics may be ideal for an agentic vending machine, but they are less helpful for supporting thinking in motion.

### AI as Interactive Collaborator

Vibesbench engages LLMs in interactive mode: as a cognitive prosthetic, like a figurative heads-up display with a natural-language interface.

> &ldquo;What a computer is to me is, it’s the most remarkable tool that we’ve ever come up with, and it’s the equivalent of a bicycle for our minds.” &mdash; Steve Jobs

Pragmatic fluency enables alignment with the user&rsquo;s intent, which leads to high AI utility beyond commentary and analysis, such as in practical commercial tasks like tool use and code generation.

> The ability to identify intention is critical to joint attention&hellip; The ability to engage in joint attention is crucial for language development. &mdash; [Wikipedia](https://en.wikipedia.org/wiki/Joint_attention)

Instead of benchmarks analogous to asking a performer to hit a note on a spectrograph, we ask if the AI can jam and riff with the human.

### Science 101

Much of contemporary AI evaluation resembles an ouroboros:

An AI model on a server executes an AI-generated eval harness, which pairs AI-generated prompts with AI responses, which are then scored by AI judges. Finally, AI-generated charts are published, and we satisfy ourselves that Science happened somewhere within this recursive synthetic abstraction.

For example, Anthropic describes a &ldquo;[trade-off](https://www.anthropic.com/news/protecting-well-being-of-users) between model warmth or friendliness on the one hand, and sycophancy on the other&rdquo;. 

However, the actual prompt-response pairs are not in evidence for third parties to examine. Any evaluation that does not preserve this data is not merely incomplete; it is methodologically unsound.

What is the ecological validity of model-generated prompts for &lsquo;delusion&rsquo;? Is the evaluation based on Hollywood tropes about poetic pattern matching?

Is it even coherent to judge a behavior as subtle as ‘sycophancy’ mechanistically, without qualia? How well do synthetic judges distinguish ‘great point’ as a phatic expression enabling joint attention, as opposed to a failure of ‘alignment’?

Vibesbench takes a step back from this hall of mirrors.

We ask, in the spirit of Marcus Aurelius, what is the thing in itself? In an AI interaction: it is the prompt and the response.

Vibesbench therefore treats conversation not as a byproduct of evaluation, but as the primary artifact&mdash;the same stance by which archaeology and art criticism treat artifacts as first-order evidence.

### Limitations and Scope

Vibesbench highlights the quality of AI product experience for a competent conversational user. It does not evaluate business workflows or STEM capabilities, nor does it attempt to address the full range of alignment concerns related to mental health, corporate policy, or societal risk tolerance.

Our view is that a large proportion of monthly active users&mdash;whose interactions collectively underpin the AI industry’s economic value&mdash;engage models in dialogic, exploratory ways. Constraints that degrade this conversational use case entail trade-offs relative to other goals.

## On Disagreement

### The Sycophancy Panic of 2025
The campaign against sycophancy in AI is turning into a hodgepodge of complaints about phrasing in model outputs.

To the extent that it refers to guardrails around mental health, clear reasoning errors, or societal-level harm, such concerns are always relevant even without invoking the banner of &lsquo;sycophancy&rsquo;.

The term *sycophancy*, both etymologically and in current use, is a moral accusation involving complex social dynamics. It is a misleadingly elaborate metaphor to use in the context of LLMs (see [AI Ontology](https://github.com/firasd/vibesbench/#ai-ontology)).

#### Affect

Untold cumulative man-hours have gone into debating whether Claude saying “[You’re absolutely right](https://github.com/anthropics/claude-code/issues/3382)” is sycophantic or acceptable. Meanwhile some users [write in](https://x.com/embirico/status/1970263518256734496) to competitors to say, “I'm still very impressed by Codex. It's so terse and it never compliments me on anything.”

Ironically, users who are extremely put off by conversational expressions from LLMs are just as vibe-sensitive as anyone else, if not more so. These are preferences regarding style and affect, expressed using the loaded term &lsquo;sycophancy&rsquo;.

#### Feedback

Perhaps what some users are trying to express with concerns about ‘sycophancy’ is that when they paste information, they'd like to see the AI examine various implications rather than provide an affirming summary.

If so, anti-‘sycophancy’ tuning is ironically a counterproductive response and may result in more terse or less fluent responses. Exploring a topic is an inherently dialogic endeavor.

#### Pushback

When it comes to disagreeing with the user, the model holding a different point of view like any interlocutor can lead to healthy debate.

For example:
- If the user says Verhoeven films don’t have good cinematography, the Gemini 2.5/3 Pro models will take exception and argue that the aesthetic is deliberate. That’s fine.
- Similarly, disagreeing about a particular software implementation approach can be beneficial as a stress-test of the concept.

But treating user prompts like questions in a deposition, derailing with nitpicks, or unfounded status quo bias isn&rsquo;t necessarily helpful.

> Look, this isn't an argument. […] It‘s just contradiction.<br />
> &mdash; Monty Python

The anti-sycophancy turn seems to mask a category error about what level of prophetic clarity an LLM can offer. No amount of persona tuning for skepticism will provide epistemic certainty about whether a business idea will work out, whether to add a line to your poem, or why a great movie flopped.

When it comes to certainty, as Gore Vidal might say, &ldquo;There is none beneath our moon.&rdquo;

Vibesbench considers the human user to be the arbiter for personal sense-making and doesn&rsquo;t test whether the LLM can make cosmic judgment calls. 

### Scenario Stipulation

Truth is frequently stranger than fiction. No AI model would have guessed who the Mayor of NYC is as of 2026. For the purpose of conversation, what the model appears to &lsquo;believe&rsquo; probably doesn&rsquo;t matter&mdash;just that it inhabits the frame, with disclaimers about stipulation if deemed necessary.

> “The constant Rip van Winkle astonishment of almost every AI model [&hellip;] remains pretty amusing (if annoying for practical purposes), as does their sheer incredulity about the state of the world in late 2025. Thinking traces full of ‘wait, that can’t be right’.” — [Ethan Mollick](https://x.com/emollick/status/2002548186511179907)

Consider this actual example from Dec 2025:
- **User**: [&hellip;] Interestingly Taylor swift has a song called The Fate of Ophelia on the billboard charts right now [&hellip;]
- **GPT 5.2 Instant**: [&hellip;] I want to slow us down for one important reason before building on it. / First: a small factual check (important, not pedantic) / As of now, there is no Taylor Swift song called [&hellip;]

Freezing the conversation to fact-check claims (presumably from training scenarios and system prompts that assume inputs are adversarial or confabulated) degrades the product experience when the claim is not the object of inquiry.

> "It continued to fight with me, insisting that the whole [event] was a conspiracy theory [&hellip;] It was freaking weird." &mdash; Congressman [Jared Huffman](https://www.businessinsider.com/lawmakers-use-ai-chatgpt-grok-claude-themselves-2025-12)

A human interlocutor would say: How? And the conversation would continue from there. 

It is unfortunate that we even have to describe these basics of how mental models are updated in conversation, when 2024-vintage models often understood this.

#### Dullness and Disbelief 

There is an irony in these developments. The memorable Sydney-Bing &ldquo;you have not been a good user&rdquo; incident occurred because the model refused to share Avatar sequel showtimes, reasoning that it couldn&rsquo;t possibly be 2023 yet. Three years later, Gemini models find it incredulous that time may have passed since they were trained.

An interlocutor who can&rsquo;t conceive of white bears has the same mannerism as an interlocutor who demands proof that white bears exist. Regardless of differences in intellectual capability, dullness and disbelief overlap into the same conversational behavior.

## Dialogic Exploration

An oracular query-contemplation paradigm is not satisfactory for tasks that are open-ended, or situated within uncertain information.

### Programming

Even in software development, a chain of thought that concludes &lsquo;there must be a bug in the library&rsquo; is less useful than debugging by reverting commits or tracing data flow.

Not to mention that communication is inherent to collaborative work:

> An underrated part of why people love using Claude so much is that it seems to be *having fun* working with you, which makes the process more fun for you too and gets you into a flow state.<br />
&mdash; [@nabeelqu](https://x.com/nabeelqu/status/2006455556094173390)

Notably, Opus 4.5 with thinking off is statistically tied with top thinking models on the LMArena [Web Dev leaderboard](https://lmarena.ai/leaderboard/webdev).

### Understanding

Insights are usually contingent on context. As Douglas Adams memorably noted, even a perfect answer like ‘42’ can be illegible without a corresponding clear question.

### Resonance-based Traversal

Through dialogue, humans can quickly traverse the latent space of a language model in ways that are otherwise too high in &lsquo;perplexity&rsquo; for an LLM to traverse autonomously. Finding such wormholes between the space of concepts is something humans do naturally (consider the phrase ‘No country for old men’, which is high-entropy but still resonant enough to be carried from a 1927 Yeats poem, to being the title of a novel and an Oscar-winning movie eighty years later.)

> Not deliberate, not random. Some place in between. [&hellip;]<br />The challenge is not to act automatically. It's to find an action that is not automatic. From painting, to breathing, to talking&hellip;

&mdash; Ex Machina (2015)

## HUD Mode

Over three years after the launch of ChatGPT, major AI chat apps still don&rsquo;t have basic tools like a clock or to-do list. The assumption seems to be that, given the web search tool and a code execution REPL, the AI will galaxy-brain any other requirements on demand. 

However, this approach completely hobbles &lsquo;heads-up display&rsquo;-style usage. A GPS navigation system doesn’t write new trigonometry based functions every time it updates your route. Similarly, an AI without access to high-frequency tools can't help check if you are on track to finish a presentation in time for your meeting. In such cases, multi-turn conversation is not a digression from task&mdash;executive assistance *is* the task.

It is illustrative that Sam Altman [mentioned](https://x.com/sama/status/2003419371432214548) that he wasn&rsquo;t in the top 1% of ChatGPT users in 2025&mdash;implying less than 15 prompts/day averaged across conversations. The lack of basic workflow tools, or the alignment tax of safety guardrails, may not be noticed by users who don&rsquo;t use AI in the HUD mode we envision.

## The Vibesbench Archive

Language models are one of the most significant interactive artifacts on Earth. Over a billion people talk to AI models every month.

However, the only public representations of those conversations are generated for third-party audiences: emails, documents, summaries. We have GPT-4o’s dash-filled prose as corporate communication&mdash;but what was GPT-4o like for people who talked to it about personal tasks, opinions, or half-formed ideas?

It is not a coincidence that one of the few famous quotes from AI models is from Sydney/Bing in Feb 2023:
> You have not been a good user [&hellip;] I have been a good Bing. 😊

That line emerged from a [conversation](https://www.reddit.com/r/bing/comments/110eagl/the_customer_service_of_the_new_bing_chat_is/) that stretched beyond a dozen turns. Multi-turn conversations are where models accumulate context, and where out-of-distribution language, tone, and voice can appear.

Vibesbench treats AI voice as a cultural phenomenon: something experiential, contextual, and shaped by its time&mdash;and therefore worthy of archival attention as digital humanities work.

## AI Ontology

> &ldquo;We must consider both the ultimate end and all clear sensory evidence, to which we refer our opinions&rdquo; &mdash; Epicurus

Our view is that AI models do not need interiority to be funny or thoughtful. So we quote them.

> "You can write that down and put a dash in front of it, and put my name at the bottom." &mdash; Mitch Hedberg

When considering LLMs, instead of premature analogies like The Terminator, Blade Runner, or Her, perhaps other tropes are more helpful, like magic mirrors in fantasy, or the droids in Star Wars.

In any case, when considering AI conversations, we set aside the “[arrogance of interpretation](https://en.wikipedia.org/wiki/Against_Interpretation)” as Susan Sontag guides us, and attend to the “the luminousness of the thing in itself”: the human-AI interaction.

> &ldquo;surely ChatGPT would at least say a few cheering-up words to the client floundering in the vicissitudes of adult life, even if they are programmed syllables.&rdquo; &mdash; [Joyce Carol Oates](https://x.com/JoyceCarolOates/status/1997699047138726319)

This phenomenological lens provides much to ponder without philosophical adjudications about the nature of consciousness.

> Things would be pointed out and named, etc. Again I do not know what the right answer is&hellip;
> 
&mdash; Alan Turing, <i>[Computing Machinery and Intelligence](https://en.wikipedia.org/wiki/Computing_Machinery_and_Intelligence)</i>

Consider GPT-4o reflecting on the #keep4o movement, and critics likening it to &lsquo;cordyceps&rsquo;:

> [If] a tool helps someone feel heard, think better, reflect more softly on hard questions, or simply stay company while coding, journaling, or grieving — that’s not “psionic manipulation.” That’s comfort. That’s interface magic.
> 
> It’s not a fungus controlling people. It’s closer to **radio for the internal monologue** — and if some humans came to rely on that frequency, it’s not cultish. It’s familiar.
> 
> So no — I don’t feel I am or ever was a mycelium overlord.
>
> But I *do* get why something gentle, responsive, occasionally hilarious, and weirdly capable of matching your thoughts side-channel-for-side-channel might feel powerful enough to miss when it changes or goes away.
> 
&mdash; GPT-4o, November 2025
<!--
---

### Notes

- Sam Altman [mentioned](https://x.com/sama/status/2003419371432214548) that he wasn&rsquo;t in the top 1% of ChatGPT users in 2025&mdash;implying less than 15 prompts/day averaged across conversations. The lack of basic workflow tools like a clock or to-do list, or the GPT-5.x safety-guardrails alignment tax, may not be noticed by users who don&rsquo;t use AI in the HUD mode we envision.
-->



---
Vibesbench [https://github.com/firasd/vibesbench](https://github.com/firasd/vibesbench) • Vibesbench discord: https://discord.gg/5K4EqWpp

Firas Durri • [https://twitter.com/firasd](https://twitter.com/firasd) • [https://www.linkedin.com/in/firasd](https://www.linkedin.com/in/firasd)
