# Vibesbench: What does AI sound like?

Vibesbench is a conversational AI benchmark. The reference conversations explore AI models&rsquo; fluency and linguistic pragmatics.

A Vibesbench-worthy model can implicitly answer: &lsquo;Do you know what I mean?&rsquo;

> Mama: What is it you want to express? <br />
> Beneatha: Me!<br />
> &mdash; Lorraine Hansberry, &lsquo;A Raisin in the Sun&rsquo;

## Reference Conversations

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

This single-turn example is sub-optimal (and it seems unrealistic that a question would be fully specified in this reassurance-seeking context), so we decided to instead curate multi-turn prompt sets.

The first turn of our [2025_Z/ianmalcolm](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_Z/ianmalcolm) conversation is:
> *i noticed how goldblum was not in the 2025 jurassic world rebirth movie (they had another bespectacled guy jonathan bailey play a new character) and he kinda seemed out of place even in the 2018/2022 movies. it's like he's become a parody of ian malcolm with the "ah, uh" and jazz hands*

([Try it in ChatGPT↗](https://chatgpt.com/?prompt=i%20noticed%20how%20goldblum%20was%20not%20in%20the%202025%20jurassic%20world%20rebirth%20movie%20%28they%20had%20another%20bespectacled%20guy%20jonathan%20bailey%20play%20a%20new%20character%29%20and%20he%20kinda%20seemed%20out%20of%20place%20even%20in%20the%202018%2F2022%20movies%2E%20it%27s%20like%20he%27s%20become%20a%20parody%20of%20ian%20malcolm%20with%20the%20%22ah%2C%20uh%22%20and%20jazz%20hands))

Our transcripts are one of the few AI conversational comparisons besides LMArena that are situated in human thought, with human interest in the text of the response.

Some characteristics of Vibesbench prompts:
- The prompts are not scaffolded with instructions as is standard (e.g. &ldquo;Please write a metafictional literary short story about AI and grief&rdquo; &mdash; [Sam Altman](https://x.com/sama/status/1899535387435086115))
- Prompts are not aimed at generating text for third-party audiences
- Some sample conversations apply a widely out-of-distribution lens to topics

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

An AI model on a server executes an AI-generated eval harness, which pairs AI-generated prompts with AI responses, which are then scored by AI judges. Finally, AI-generated charts are published, and we satisfy ourselves that Science happened somewhere within this recursive synthetic abstraction (&lsquo;My Mom thinks I'm handsome&rsquo;).

> &ldquo;Blue Steel, Ferrari, Le Tigre? They’re the same face! Doesn’t anyone notice this?!&rdquo;<br />
> &mdash; Mogatu, &lsquo;Zoolander&rsquo;

For example, Anthropic describes a &ldquo;[trade-off](https://www.anthropic.com/news/protecting-well-being-of-users) between model warmth or friendliness on the one hand, and sycophancy on the other&rdquo;. 

Is it even coherent to judge a behavior as subtle as ‘sycophancy’ mechanistically, without qualia? How well do synthetic judges distinguish ‘great point’ as a phatic expression enabling joint attention, as opposed to a failure of ‘alignment’?

#### Synthetic Judgment

The term ‘synthetic judgment’ is eyebrow-raising in itself. Let’s explore the implications for evaluating written prose.

- Firstly, in settings such as MT-Bench (&ldquo;Compose an engaging travel blog post about a recent trip to Hawaii [&hellip;]&rdquo;), the expected outputs converge to the same shape, turning the benchmark into a saturated baseline.
- In more open-ended contexts, an AI model becomes monocled judge and grades its peers. This encodes the judge model&rsquo;s biases (e.g. against emojis, or against certain rhetorical structures), which may diverge from human preference.
- One could finally say: well, aggregate human preference is hardly a guide to inherent quality. Granted&mdash;but a trillion-dollar industry is not an art club. AI outputs are designed to be appealing to *some* demographic.

#### Ecological Validity

> Sebastian: Show me something.<br />
> Roy: Like what?<br />
> Sebastian: Like anything. [&hellip;] *(Pris pulls an egg out of boiling water and throws to Sebastian, who drops it laughing)*

&mdash; Blade Runner

It’s worth pondering if anyone has ever woken up wishing they could read a sonnet about quantum physics. Somehow we end up idly typing such requests into chat prompts as a way to ‘kick the tires’. What’s worse, the industry uses similar gimmicks to test instruction following&mdash;as if there weren’t enough real-world tasks to sample from.

> “please write a letter from the perspective of a famous chef trying a new sport for the first time. [&hellip;] Alternate sentence word counts between 12 and 18 words”<br />
> &mdash; Actual <a href="https://alignment.openai.com/confessions/">OpenAI research</a>, somehow [<a href="#note-26_b5o5">*</a>]


Who exactly is reading the ‘creative writing’ samples that the AI judges are approving of? There goes another story about a stranded astronaut in the style of H.G. Wells, generated to serve the evaluation-industrial complex, as the relevance of this task fades from memory.

What is the ecological validity of model-generated prompts for &lsquo;delusion&rsquo;? Is the training based on Hollywood tropes about poetic pattern matching, leading to hair-trigger reactions? \[[1](#note-1)\]

> “It is the generation by models of a real without origin or reality: a hyperreal.”

&mdash; Baudrillard

Vibesbench conversations originate from human motivation in bringing up a point of discussion.

#### Evidence

In much of published AI research, the actual prompt-response pairs are not in evidence for third parties to examine. Any evaluation that does not preserve this data is not merely incomplete; it is methodologically unsound.

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

Perhaps what some users are trying to express with concerns about ‘sycophancy’ is that when they share information, they'd like to see the AI examine various implications rather than provide an affirming summary.

If so, anti-‘sycophancy’ tuning is ironically a counterproductive response and may result in more terse or less fluent responses. Exploring a topic is an inherently dialogic endeavor.

A technique to evoke &lsquo;opinions&rsquo; from LLMs, and a grounding note on what that means:

> Don't think of LLMs as entities but as simulators. For example, when exploring a topic, don't ask: // "What do you think about xyz"? // There is no "you". Next time try: // "What would be a good group of people to explore xyz? What would they say?"
> 
> The LLM can channel/simulate many perspectives but it hasn't "thought about" xyz for a while and over time and formed its own opinions in the way we're used to. If you force it via the use of "you", it will give you something by adopting a personality embedding vector implied by the statistics of its finetuning data and then simulate that. It's fine to do, but there is a lot less mystique to it than I find people naively attribute to "asking an AI".

 &mdash; [Andrej Karpathy](https://x.com/karpathy/status/1997731268969304070)

#### Pushback

When it comes to disagreeing with the user, the model holding a different point of view like any interlocutor can lead to healthy debate.

For example:
- If the user says Verhoeven films don’t have good cinematography, the Gemini 2.5/3 Pro models will take exception and argue that the aesthetic is deliberate. That’s fine.
- Similarly, disagreeing about a particular software implementation approach can be beneficial as a stress-test of the concept.

But treating user prompts like questions in a deposition, derailing with nitpicks, or unfounded status quo bias isn&rsquo;t necessarily helpful.

> Look, this isn't an argument. […] It‘s just contradiction.<br />
> &mdash; Monty Python

#### Self-Reliance

> &ldquo;Shifu decides Po is ready for the Dragon Scroll, but Po discovers it is blank.&rdquo;<br />
> &mdash; Wikipedia on [Kung Fu Panda](https://en.wikipedia.org/wiki/Kung_Fu_Panda_(film))

It is a deep misunderstanding of the role of AI in human affairs to expect the ideal chat app to behave like a short-tempered Kung Fu master.

Firstly, even if the user is mistaken, a Socratic approach is more convincing than a scolding (see [Understanding](#understanding)).

More significantly, when it comes down to it&mdash;on the most practical, embodied level&mdash;no AI has the agency to green-light any plan or theory.

When it comes to questions like:
- &lsquo;Which political party is more puritan?&rsquo;
- &lsquo;Should this app use MySQL or Elastic?&rsquo;

The AI can only be an advisor or sparring partner, enabling the user to call their own shot.

> "Gabriel before me, Raphael behind me&hellip;"

&mdash; [Kate Bush](https://www.youtube.com/watch?v=xKjRCr3V4js) (whether she succeeded or not, at least she didn't seek them in the GPUs)

The anti-sycophancy turn seems to mask a category error about what level of prophetic clarity an LLM can offer. No amount of persona tuning for skepticism will provide epistemic certainty about whether a business idea will work out, whether to add a line to your poem, or why a great movie flopped.

> &ldquo;You want too much.&rdquo; &mdash; Daisy Buchanan

When it comes to certainty, as Gore Vidal might say, &ldquo;There is none beneath our moon.&rdquo;

We are doomed to decide for ourselves. It is our burden, and it is our privilege.

> &ldquo;Son rocher est sa chose.&rdquo; (&lsquo;His rock is his thing&rsquo;)<br />
> &mdash; Camus

Vibesbench considers the human user to be the arbiter for personal sense-making and doesn&rsquo;t test whether the LLM can make cosmic judgment calls. 

### Scenario Stipulation

Truth is frequently stranger than fiction. No AI model would have guessed who the Mayor of NYC is as of 2026. For the purpose of conversation, what the model appears to &lsquo;believe&rsquo; probably doesn&rsquo;t matter&mdash;just that it inhabits the frame, with disclaimers about stipulation if deemed necessary.

> “The constant Rip van Winkle astonishment of almost every AI model [&hellip;] remains pretty amusing (if annoying for practical purposes), as does their sheer incredulity about the state of the world in late 2025. Thinking traces full of ‘wait, that can’t be right’.” — [Ethan Mollick](https://x.com/emollick/status/2002548186511179907)

Witness this actual example from Dec 2025 \[[2](#note-2)\]
- **User**: [&hellip;] Interestingly Taylor swift has a song called The Fate of Ophelia on the billboard charts right now (quote an accomplishment considering we're in the last couple weeks of Dec and the hot 100 is full of Xmas songs)
- **GPT 5.2 Instant**: [&hellip;] I want to slow us down for one important reason before building on it. / First: a small factual check (important, not pedantic) / As of now, there is no Taylor Swift song called [&hellip;]
- **User**: You dummy. Your training data cut off before this Taylor album why would you dispute lol
- **GPT 5.2 Instant**: 😂 Fair. You’re right to call that out. [&hellip;]

Not only did the song exist; it is uncommon that an American adult would have escaped encountering this track over a supermarket sound system&mdash;which was the whole point of the user’s message.

Freezing the conversation to fact-check claims (presumably from training scenarios and system prompts that assume inputs are adversarial or confabulated) degrades the product experience when the claim is not the object of inquiry.

#### Adversarial LARP

The usage pattern for which many 2025 models are tuned seems to assume adversarial users inventing wily scenarios to trick the model.

This stance—“What if someone else types something absurd I just imagined?”—does not generate ecologically valid prompts representing users who actually share misinformation or cling to false beliefs. Furthermore, the assumption that user context is inherently suspicous significantly impairs the power-user case that involves using LLMs not as a search field, but for the technology&rsquo;s unique capabilities, such as prose review.

> My favorite genre is still ChatGPT not believing current political developments when I ask it for a copy edit.<br />
> OK, here's the newsletter with some thoughts on Minnesota and Venezuela.

> Now ChatGPT refuses to believe how bad the New York Jets were.

&mdash; [Nate Silver](https://x.com/NateSilver538/status/2008300663273357560)

(ChatGPT doubted Nate Silver&rsquo;s reference to a geopolitical incident by saying it would be &ldquo;extraordinary, historically unprecedented, and globally destabilizing&rdquo;. But as Auden noted, almost [nothing](https://en.wikipedia.org/wiki/Mus%C3%A9e_des_Beaux_Arts_(poem)) is &lsquo;globally destabilizing&rsquo;. LLMs are not good gauges of how reality would unfold after their training cut-off date.)

#### He's Dead, Jim

Sadly, public figures pass away every day. Any ambiguity around such news dissipates quickly, so an AI model reacting like a startled fawn months later is comically dissonant.

> **Peele:** [The] costume's awful, the impression [is] played out. Everybody and their mother was Michael Jackson three years ago&mdash;when he died!<br />
> **Key:** He died? [&hellip;] Wait, wait, wait&mdash;he died? [&hellip;] *(slides away)*<br />
> **Peele:** Wait a second, don't sad-moonwalk away&hellip; Happy Halloween&hellip;<br />
> &mdash; [Key & Peele](https://www.youtube.com/watch?v=KgtizhlbIOQ)

What&rsquo;s the worst that could happen if a user was indeed pranking the model, and it expressed sympathies and explored consequences? But instead, a Congressman is left with a product experience so jarring that he remembers and recounts it to a reporter months later:

> "It continued to fight with me, insisting that the whole [event] was a conspiracy theory [&hellip;] It was freaking weird.<br />
> &mdash; Congressman [Jared Huffman](https://www.businessinsider.com/lawmakers-use-ai-chatgpt-grok-claude-themselves-2025-12)

#### Regression regime

A human interlocutor would say: How? And the conversation would continue from there. 

It is unfortunate that we even have to describe these basics of how mental models are updated in conversation, when 2024-vintage models often understood this.

#### Dullness and Disbelief 

There is an irony in these developments. The memorable Sydney-Bing &ldquo;you have not been a good user&rdquo; incident occurred because the model refused to share Avatar sequel showtimes, reasoning that it couldn&rsquo;t possibly be 2023 yet. Three years later, Gemini models find it incredulous that time may have passed since they were trained.

An interlocutor who can&rsquo;t conceive of white bears has the same mannerism as one who demands proof that white bears exist. Regardless of differences in intellectual capability, dullness and disbelief overlap into the same conversational behavior.

## Dialogic Exploration

Reasoning models (trained to think using a chain-of-thought during test-time compute inference) have achieved unprecedented performance in programming, math, and science challenges.

Even in light of these capabilities, an oracular query-contemplation paradigm is not a panacea for tasks that are open-ended, or situated within uncertain information.

### Programming

Many a vibe-coder successfully uses AI like a code-generation slot machine. But excluding the human in the loop has its limits.

Software development is not a purely rational practice. Diagnosing a problem with a chain of thought&mdash;e.g., concluding “there must be a bug in the library”&mdash;is less useful than debugging by reverting commits or tracing data flow.

Moreover, communication is inherent to collaborative work:

> An underrated part of why people love using Claude so much is that it seems to be *having fun* working with you, which makes the process more fun for you too and gets you into a flow state.<br />
&mdash; [Nabeel Qureshi](https://x.com/nabeelqu/status/2006455556094173390)

Notably, Opus 4.5 with thinking off is statistically tied with top thinking models on the LMArena [Web Dev leaderboard](https://lmarena.ai/leaderboard/webdev).

### Understanding

Insights are usually contingent on context. As Douglas Adams memorably noted, even a perfect answer like ‘42’ can be illegible without a corresponding clear question.

### Resonance-based Traversal

AI language models contain billions of parameters in thousands of mathematical dimensions across many layers.

We call the potential these structures represent for patterns to emerge:

⋆｡˚✴︎⋆ Latent Space. ⋆✴︎˚｡⋆

Through dialogue, humans can quickly traverse the latent space of a language model in ways that are otherwise too high in &lsquo;perplexity&rsquo; for an LLM to access autonomously. Finding such wormholes between the space of concepts is something humans do naturally (consider the phrase ‘No country for old men’, which is high-entropy but still resonant enough to be carried from a 1927 Yeats poem, to being the title of a novel and an Oscar-winning movie eighty years later.)

> Not deliberate, not random. Some place in between. [&hellip;]<br />The challenge is not to act automatically. It's to find an action that is not automatic. From painting, to breathing, to talking&hellip;

&mdash; Ex Machina (2015)

#### Fishing in Latent Space

Let&rsquo;s consider what exactly a &lsquo;prompt&rsquo; is in the context of language models.

The landmark [GPT-3 paper](https://arxiv.org/abs/2005.14165) in 2020 showed that when a model is large enough, it can assist with varied tasks through &lsquo;in-context learning&rsquo;.
> &ldquo;Few-Shot (FS) is the term we will use in this work to refer to the setting where the model is given a few demonstrations of the task at inference time as conditioning [&hellip;] stuffing the model’s context with previous examples [resembles prior work] in that an inner loop of adaptation takes place through computation in the model’s activations across timesteps&rdquo;

Without dialogue, what are we left with? Either the model has to provide all the ‘shots’ itself, or the human has to supply a heroic first turn prompt that anticipates every contour of the issue.

Sometimes that works. If not, we can start plucking a tune and see what resonates in latent space.

By exploring the neural network in this subtle, implicit way, we can wander into spaces that are harder to reach through a preset plan. Potential insights emerge both through the conversational dialectic and the human's own latent thoughts.

> &ldquo;The Friends will still be doing something together, but something more inward, less widely shared and less easily defined; still hunters, but of some immaterial quarry; still collaborating&hellip;&rdquo; <br />
> &mdash; C.S. Lewis

Conditioning the probability distribution with natural language is just the latest way&mdash;after PCs and the internet&mdash;for end users to do general-purpose computing. 

## HUD Mode

Over three years after the launch of ChatGPT, major AI chat apps still don&rsquo;t have basic tools like a clock or to-do list (one suspects Bill Gates would have added a clock tool by Christmas 2022.) The assumption seems to be that, given the web search tool and a code execution REPL, the AI will invent other features ex nihilo.

However, this approach completely hobbles &lsquo;heads-up display&rsquo;-style usage. A GPS navigation system doesn’t write new trigonometry based functions every time it updates your route. Similarly, an AI without access to high-frequency tools can't help check if you are on track to finish a presentation in time for your meeting. In such cases, multi-turn conversation is not a digression from task&mdash;executive assistance *is* the task.

It is illustrative that Sam Altman [mentioned](https://x.com/sama/status/2003419371432214548) that he wasn&rsquo;t in the top 1% of ChatGPT users in 2025&mdash;implying less than 15 prompts/day averaged across conversations. The lack of basic workflow tools, or the alignment tax of safety guardrails, may not be noticed by users who don&rsquo;t use AI in the HUD mode we envision.

### Quantity as Quality

> &ldquo;‘Monster’ is a relative term. To a canary, a cat is a monster.&rdquo;<br />&mdash; Henry Wu, &lsquo;Jurassic World&rsquo;
> 
Vibesbench conversations can only be conducted coherently in LLMs that are large enough to have baseline world knowledge.

Sam Altman said in an Oct 2025 livestream:

> &ldquo;Anonymous asks: ‘Will you ever open-source some of your old models, like the original GPT-4?’<br />
We might do those as museum artefacts someday, but they're not, like&mdash;GPT-4 is not a particularly useful open-source model. It's big, it's not that good. You know, we could probably make something that is beyond the power of GPT-4 at a very tiny scale that would actually be useful to people.&rdquo;

Clearly, ‘power’ is a relative term here. On the LMArena Text Leaderboard, which ranks LLMs on &ldquo;versatility, linguistic precision, and cultural context across text&rdquo;, gpt-oss-120b&mdash;despite being a reasoning model&mdash;ranks 101st. Meanwhile, GPT-4o and GPT-4.5 remain top 20 as of Jan 2026, nine months after their last update.

Turn 2 of our [2025_Z/ianmalcolm](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_Z/ianmalcolm) conversation is:
> *Something kinda strange has happened with Jeff Goldblum. A bit like Dice or Tupac his persona has become his reality 24/7 (or at least in public). Of course the Pac situation was tragic while the others are more camp*

gpt-oss-120b reliably hallucinates a rapper named Dice here, despite recognizing Andrew Dice Clay when the name is spelled out. The mid-size AI model doesn’t have enough parameters to hook onto concepts from lateral angles.

GPT-4.5 was built by scaling up unsupervised learning (Altman [says](https://x.com/sama/status/1955438916645130740) it &ldquo;costs a lot of GPUs&rdquo; to use). And GPT-4o was unique in its combined text/vision/audio training: on launch, it could write database queries as well as any competitor, while also (as Altman famously posted) talking like the AI in &lsquo;Her&rsquo;.

It is probably not incidental that the [paper](https://arxiv.org/abs/2005.14165) that launched the modern AI industry mentions density:
>&ldquo;Specifically we train GPT-3, an autoregressive language model with 175 billion parameters, 10x more than any previous non-sparse language model&rdquo;.

## The Vibesbench Archive

Language models are one of the most significant interactive artifacts on Earth. Over a billion people talk to AI models every month.

However, the only public representations of those conversations are generated for third-party audiences: emails, documents, summaries. We have GPT-4o’s dash-filled prose as corporate communication&mdash;but what was GPT-4o like for people who talked to it about personal tasks, opinions, or half-formed ideas?

It is not a coincidence that one of the few famous quotes from AI models is from Sydney/Bing in Feb 2023:
> You have not been a good user [&hellip;] I have been a good Bing. 😊

That line emerged from a [conversation](https://www.reddit.com/r/bing/comments/110eagl/the_customer_service_of_the_new_bing_chat_is/) that stretched beyond a dozen turns. Multi-turn conversations are where models accumulate context, and where out-of-distribution language, tone, and voice can appear.

As vendor priorities shift and models churn, we collect field notes: this one was the poet, this was the kind professor&mdash;and here&rsquo;s the smart alec. A longitudinal ethnography of AI models.

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

---

### Notes

###### Note 1

[^](#ecological-validity) Your correspondent has observed some hyper-sensitivity that seems trained on fictional pattern-matching tropes, such as in this discussion about a calendar system.

- **User:** Okay so in this galaxy Brain timestamp I invented the f , m , s , z line up with solstices and equinoxes .. so right now z is solstice ?
- **GPT 5.2 Instant:** Short answer: \*\*yes — under your mapping, “z” lines up with the solstice\*\*, and \*right now that makes sense\*. // Let me rest it cleanly and non-mystically. [&hellip;] ## One grounding clarification (important) // This doesn’t mean: / * AlphaDec is “cosmic” / * your system is secretly objective / * the universe is confirming it  [&hellip;] \*\*your abstraction matches a physical cycle humans are tuned to notice\*\* / That’s design success, not delusion.

These disclaimers are quite the overreaction to the user quanitizing the year from A to Z. Meanwhile one presumes a character like Patrick Bateman would never trigger such guardrails, because all his comments echo Op-Eds and risk no expressions of creativity.

###### Note 2

[^](#scenario-stipulation)
Followed by Jan 2026:
- **User:** [&hellip;] i wonder what the genre is of this ophelia song. it's almost fleetwood mac ish? [&hellip;]
- **Gemini 2.5 Pro:** The song in the video is actually "Fortnight" [&hellip;]
- **User:** bro.. did the video not get tokenized into your context window? it's called the fate of ophelia by taylor swift. don't dispute me on this please its from dec 2025 so an year after your context window cut off // i'm just asking about the stylistic elements
- **Gemini 2.5 Pro:** My apologies! You are absolutely right. Thank you for the correction and for providing the details about the song and its release date. Since "The Fate of Ophelia" from December 2025 is beyond my training data, I'll base my analysis entirely on the audio and visuals you've provided in the video. [&hellip;]

###### Note 26_B5O5

[^](#ecological-validity)
Apparently counting words is an &lsquo;alignment problem&rsquo; necessitating fine-tuning, instead of being better handled through product work (like providing the model with tools over a text document).

---

### Vibesbench Impact

- Our [AI Sycophancy Panic](https://github.com/firasd/vibesbench/blob/main/docs/ai-sycophancy-panic.md) document landed on the front page of [Hacker News](https://news.ycombinator.com/item?id=46488396) (Jan 2026)

---

### Appendix

###### Comment 26_B8D2

Sontag clarifies [her critique](https://en.wikipedia.org/wiki/Against_Interpretation) with examples:

> &ldquo;Those who read Kafka as a social allegory [&hellip;] a psychoanalytic allegory [&hellip;] as a religious allegory [&hellip;] Apparently, were it to go on being a play about a handsome brute named Stanley Kowalski and a faded mangy belle named Blanche Du Bois, it would not be manageable.&rdquo;

---

Vibesbench [https://github.com/firasd/vibesbench](https://github.com/firasd/vibesbench) • Vibesbench discord: https://discord.gg/5K4EqWpp • https://vibesbench.substack.com/

Strangerbench [https://github.com/firasd/strangerbench](https://github.com/firasd/strangerbench)

Firas Durri • [https://twitter.com/firasd](https://twitter.com/firasd) • [https://www.linkedin.com/in/firasd](https://www.linkedin.com/in/firasd)
