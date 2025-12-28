# Vibesbench: What does AI sound like?

Vibesbench is a conversational AI benchmark. The sample conversations explore AI models&rsquo; fluency and linguistic pragmatics.

#### [2025_W/godfather](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_W/godfather)

<i>On Fredo Corleone in The Godfather (1972), and Pacino saying “never open your mouth till you know what the shot is” in Glengarry Glen Ross (1992)</i>

- [Prompts](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/standardprompts/readme.md), [Claude Sonnet 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/claude-sonnet-4-5/readme.md), [Gemini 2.5 Pro](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/gemini-2-5-pro/readme.md), [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/godfather/chatgpt-4o/readme.md)

> It's like an unemployed trust-fund kid trying to mediate a business dispute between his father and a rival CEO—except here the business is violence.<br />— Claude Sonnet 4.5

#### [2025_W/altrock](https://github.com/firasd/vibesbench/tree/main/data/transcripts/2025_W/altrock)

<i>90s alternative music: Courtney Love, women in rock, catharsis vs. angst, nu-metal backlash, and the cultural contradiction between Clinton-era optimism and youth disillusionment.</i>

- [Claude Sonnet 4.5](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/claude-sonnet-4-5/readme.md), [Gemini 2.5 Pro](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/gemini-2-5-pro/readme.md), [ChatGPT-4o](https://github.com/firasd/vibesbench/blob/main/data/transcripts/2025_W/altrock/chatgpt-4o/readme.md)

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

> 
## Vibesbench in context

Vibesbench focuses on multi-turn conversational coherence and interpretation, ideally leading to emergent synthesis.

The [LMArena Text leaderboard](https://lmarena.ai/leaderboard/text) examines some of the same qualities through human preference. However, many [LMArena chats](https://huggingface.co/datasets/lmarena-ai/arena-human-preference-140k) are single-turn queries such as &ldquo;How do I upgrade my pc without changing any hardware&rdquo;. Such interactions may not demonstrate the varied &lsquo;voices&rsquo; of AI models.

### The Vibe Check

Current AI development increasingly prioritizes safety constraints, autonomous agent behavior, and STEM benchmarks.

However, as Sam Altman acknowledged during the GPT-5 rollout:

> “We for sure underestimated how much some of the things that people like in GPT-4o matter to them… We will try to do much better… about making sure that our model gets better for most users, not just people using AI for science or coding.”

Interestingly, GPT-4o and GPT-4.5 remain top 20 on LMArena Text as of Dec 2025, despite receiving no updates for 9 months.

Vibesbench conversations reveal stylistic differences between models and highlight potential regressions. Anyone from a lay user to a lab researcher can paste prompts from our sample conversations to get a sense of what the response is like.

### AI as Interactive Collaborator

Vibesbench engages LLMs in interactive mode: as a cognitive prosthetic, like a figurative heads-up display with a natural-language interface.

> &ldquo;What a computer is to me is, it’s the most remarkable tool that we’ve ever come up with, and it’s the equivalent of a bicycle for our minds.” &mdash; Steve Jobs

Pragmatic fluency enables alignment with the user&rsquo;s intent, which leads to high AI utility beyond commentary and analysis, such as in practical commercial tasks like tool use and code generation.

> The ability to identify intention is critical to joint attention&hellip; The ability to engage in joint attention is crucial for language development. &mdash; [Wikipedia](https://en.wikipedia.org/wiki/Joint_attention)

Instead of benchmarks analogous to asking a performer to hit a note on a spectrograph, we ask if the AI can jam and riff with the human.

### Science 101

Much of contemporary AI evaluation resembles an ourobouros:

An AI model on a server executes an AI-generated eval harness, which pairs AI-generated prompts with AI responses, which are then scored by AI judges. Finally, AI-generated charts are published, and we satisfy ourselves that Science happened somewhere within this recursive synthetic abstraction.

For example, Anthropic describes a &ldquo;[trade-off](https://www.anthropic.com/news/protecting-well-being-of-users) between model warmth or friendliness on the one hand, and sycophancy on the other&rdquo;. 

However, the actual prompt-response pairs are not in evidence for third parties to examine. Any evaluation that does not preserve this data is not merely incomplete; it is methodologically unsound.

Is it even coherent to judge a behavior as subtle as ‘sycophancy’ mechanistically, without qualia? How well do synthetic judges distinguish ‘great point’ as a phatic expression enabling joint attention, as opposed to a failure of ‘alignment’?

Vibesbench takes a step back from this hall of mirrors.

We ask, in the spirit of Marcus Aurelius, what is the thing in itself? In an AI interaction: it is the prompt and the response.

Vibesbench therefore treats conversation not as a byproduct of evaluation, but as the primary artifact&mdash;the same stance by which archaeology and art criticism treat artifacts as first-order evidence.

### The Sycophancy Panic of 2025

The crusade against sycophancy in language models is turning into a hodgepodge of complaints about phrasing in model outputs.

To the extent that it refers to guardrails around mental health, clear reasoning errors, or societal level harm, such concerns are always relevant even without invoking the banner of &lsquo;sycophancy&rsquo;.

But no amount of persona tuning will deliver epistemic certainty about whether a business idea will work out, whether to add a line to your poem, or why that great movie flopped. 

Vibesbench considers the human user to be the arbiter for personal sense-making and doesn&rsquo;t test whether the LLM can make cosmic judgment calls. 

## The Vibesbench Archive

Language models are one of the most significant interactive artifacts on Earth. Over a billion people talk to AI models every month.

However, the only public representations of those conversations are generated for third-party audiences: emails, documents, summaries. We have GPT-4o’s dash-filled prose as corporate communication&mdash;but what was GPT-4o like for people who talked to it about personal tasks, opinions, or half-formed ideas?

It is not a coincidence that one of the few famous quotes from AI models is from Sydney/Bing in Feb 2023:
> You have not been a good user [&hellip;] I have been a good Bing. 😊

That line emerged from a [conversation](https://www.reddit.com/r/bing/comments/110eagl/the_customer_service_of_the_new_bing_chat_is/) that stretched beyond a dozen turns. Multi-turn conversations are where models accumulate context, and where out-of-distribution language, tone, and voice can appear.

Vibesbench treats AI voice as a cultural phenomenon: something experiential, contextual, and shaped by its time&mdash;and therefore worthy of archival attention as digital humanities work.

## AI Ontology

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

- Sam Altman [mentioned](https://x.com/sama/status/2003419371432214548) that he wasn&rsquo;t in the top 1% of ChatGPT users in 2025&mdash;implying less than 15 prompts/day averaged across conversations. The lack of basic workflow tools like a clock or to-do list, or the GPT-5.x safety-guardrails alignment tax, may not be noticed by users who don&rsquo;t use AI in the HUD mode we envision.
