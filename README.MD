<div align="center">

# Aria Han

**AI Systems Architect · Writer**

<a href="https://ariaxhan.com"><img src="https://img.shields.io/badge/ariaxhan.com-000000?style=for-the-badge&logo=About.me&logoColor=white" alt="Website" /></a>
<a href="https://medium.com/@ariaxhan"><img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium" /></a>
<a href="https://github.com/ariaxhan"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://linkedin.com/in/ariahan"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

</div>

---

I build systems that make AI agents predictable. Not smarter. Predictable.

Agents fail when they have to guess. The fix isn't better prompts; it's better contracts. Explicit scope. Typed learnings. Tiered routing based on complexity. The agent doesn't interpret. It executes against constraints.

Systems architecture applied to language models. Poet's precision for the prompts; engineer's rigor for the infrastructure.

---

## Recent

**[Stop Copying Other People's AI Setups. Build One That's Actually Yours.](https://medium.com/@ariaxhan/stop-copying-other-peoples-ai-setups-build-one-that-s-actually-yours-e1a05ebabc2a)**

A rule you copied never had to prove itself to you. Extract every rule as a falsifiable hypothesis, mine your own session history for evidence, score it against a standard set in advance, keep only what survives. Most popular workflows don't.

**[What an AI Detector Actually Measures](https://medium.com/@ariaxhan/what-an-ai-detector-actually-measures-86b452979a5a)**

AI detectors measure predictability, not authorship. Low perplexity flags machine writing, careful human prose, and familiar phrasing identically — a false-alarm rate far past the advertised number. A tool that can't define its own score is very confident about something it can't measure. People lose jobs over it.

**[Opus 4.8 vs 4.7 vs Sonnet vs Haiku](https://medium.com/@ariaxhan/opus-4-8-vs-4-7-vs-sonnet-vs-haiku-when-the-expensive-model-is-worth-it-44892a75d5c5)**

Twenty-one real tasks across every tier. For extraction and writing, the cheap models land within a hair of Opus at a fraction of the cost. Reaching for the biggest model by default is the most expensive habit in AI — reserve it for genuinely multi-step reasoning, not everything.

---

## The Thesis

**Agents need constraints, not capability.**

Most AI workflows operate on vibes. You describe a task. The agent interprets. If the output matches what you imagined, ship it. If not, iterate until exhausted.

I build systems that eliminate the interpretation step:

- **Contracts before code**: Explicit acceptance criteria, scope boundaries, failure conditions. Written before implementation, not discovered during review.
- **Learnings as database objects**: Not notes. Typed rows: failures, patterns, gotchas. Queryable by category. Evidence-gated. Surviving session boundaries.
- **Tiered routing**: Complexity determines pipeline. 1-2 files: execute directly. 3-5 files: contract required. 6+: full verification with adversarial QA.

The agents aren't getting smarter. They're getting access to what their predecessors learned. That turns out to be enough.

---

## Research

I measure how models compute, not whether they're correct.

**[latent-diagnostics](https://github.com/ariaxhan/latent-diagnostics)**: Representation-level analysis of LLMs via SAE attribution graphs. Grammar tasks show d=1.08 higher influence than reasoning tasks. After length control, genuine computational regime differences emerge.

**[universal-spectroscopy-engine](https://github.com/ariaxhan/universal-spectroscopy-engine)**: Treats LLM activations as light spectra. 52% reduction in SAE reconstruction loss with structured vs natural language syntax. LLMs are vector computers pretending to be text processors.

**[experiments](https://github.com/ariaxhan/experiments)**: Append-only specimen archive for LLM experiments.

---

## Production

| | |
|---|---|
| **[Brink](https://github.com/ariaxhan/brink-mind)** | iOS journaling with private AI and biometrics. SwiftUI, HealthKit. |
| **HeyContent** | Content management for creators. Cross-platform insights, conversational persona generation. |
| **ModelMind** | Duolingo-style app for genuinely understanding how AI works — not how to prompt it, how it thinks. In development. |

---

## Infrastructure

| | |
|---|---|
| **[KERNEL](https://github.com/ariaxhan/kernel-claude)** | Claude Code that learns from itself. SQLite-backed agent memory, multi-agent orchestration, and an experiment engine that proves which workflows actually hold up. Active development, open source. [Cursor version](https://github.com/ariaxhan/kernel-cursor). |
| **[conductor](https://github.com/ariaxhan/conductor)** | MCP server bridging Claude Desktop and Claude Code. |
| **[metabrain](https://github.com/ariaxhan/metabrain)** | Zero-dependency SQLite memory layer for AI agents. The "Stop Writing Markdown" architecture as a drop-in library. |
| **[memory-pool](https://github.com/ariaxhan/memory-pool)** | Memory isn't a timeline. Structured architecture for persistent AI context. |
| **[event-horizon](https://github.com/ariaxhan/event-horizon)** | Physics-informed encryption. SYK scrambling, chimera camouflage, resonance locking. |

---

## Writing

*Currently writing **Intelligence Architecture** — a principles-first book on building with AI. In progress.*

[Engineering the Soul](https://medium.com/@ariaxhan/engineering-the-soul-49428c073c4e): AI consciousness read through four novels. Every answer sounds like the person asking the question.

[The Agent-Ready Web](https://medium.com/@ariaxhan/the-agent-ready-web-a-working-guide-to-cloudflares-new-score-1ed0fce8d760): Making a site legible to AI agents — llms.txt, MCP, markdown negotiation, content-signals. Half the checks are policy, not config.

[Self-Learning Agent Civilization](https://medium.com/@ariaxhan/how-i-turned-cursor-into-a-self-learning-agent-civilization-7a149e6f34e8): The original system that started everything.

[Stop Building Chatbots](https://medium.com/@ariaxhan/part-1-stop-building-chatbots-why-we-killed-the-conversation-to-fix-ai-698641d5cfa2): Why the chat interface is a dead end.

[How to Make Claude Code Actually Work](https://medium.com/@ariaxhan/how-to-make-claude-code-actually-work-structure-memory-and-multi-agent-workflows-6d32b1d815d2): The full guide to KERNEL — structure, memory, and multi-agent workflows.

[KERNEL](https://medium.com/@ariaxhan/kernel-the-ultimate-self-evolving-claude-code-and-cursor-configuration-system-a3ddeb7f4d32): Configuration that adapts as you work.

[Semantic Drift is Quantum Decoherence](https://medium.com/@ariaxhan/semantic-drift-is-just-quantum-decoherence-cec24b0fb4a4): Multi-agent coordination through physics.

[Why Prompt Engineering Can't Fix Hallucinations](https://medium.com/@ariaxhan/why-prompt-engineering-cant-fix-hallucinations-but-neurosurgery-can-a1a7afa2f8bf): The case for mechanistic intervention.

---

```
Python · TypeScript · Swift
FastAPI · Next.js · SvelteKit
Claude · SAEs · Modal
```

<div align="center">

San Francisco

<a href="mailto:ariaxhan@gmail.com"><img src="https://img.shields.io/badge/ariaxhan@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a> <a href="https://x.com/aria__han"><img src="https://img.shields.io/badge/@aria__han-1DA1F2?style=flat-square&logo=twitter&logoColor=white" alt="X" /></a>

</div>
