<div align="center">

# Aria Han

**Poet. Programmer. Prompt Architect.**

*Building production AI systems through language, not just code.*

<a href="https://ariaxhan.com"><img src="https://img.shields.io/badge/ariaxhan.com-000000?style=for-the-badge&logo=About.me&logoColor=white" alt="Website" /></a>
<a href="https://github.com/ariaxhan"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://medium.com/@ariaxhan"><img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium" /></a>
<a href="https://linkedin.com/in/ariahan"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>

</div>

---

## Philosophy

I was an English major before I ever wrote code. That's not a disclaimer; it's the point.

After a year building production systems with AI (10-12 hours daily, 7 days a week), I've learned: **language is the key variable in a Large Language Model**. LLMs aren't code generators. They're readers. What you write shapes what they do. This makes writing skill the primary variable in AI-assisted development, not programming knowledge.

The industry hasn't caught up. Most developers treat prompting as an afterthought. I treat it as craft. The same craft I spent years developing as a writer, a poet, an English major obsessed with precision. Now that craft builds production systems.

**Code is just another language.** Reading it is like reading a book. Just as fun. Just as natural. I'm not limited by decades of singular experience in computer science. I can think of brand new solutions because I come from somewhere else. And now that coding is no longer about writing code but writing natural language, that somewhere else is exactly where you want to be.

---

## Core Principles

```
CORRECTNESS > SPEED
One working implementation beats three debug cycles.
Aim for zero debugging. Get it right the first time.
Even if planning takes twice as long, that's where the time should go.

EVERY LINE IS A LIABILITY
Someone (probably you) will have to debug it later.
AI takes the happy path; you have to design the structure that prevents spaghetti.
Config > code. Native > custom. Existing > new.

RESEARCH FAILURES, NOT SOLUTIONS
Search for first-hand accounts of what broke.
Don't waste time making mistakes someone already posted on StackOverflow.
AI doesn't know specifics. MCP servers, docs, real research do.

CONTEXT IS EVERYTHING
Lean context prevents rot. Monitor it. Manage it.
Fresh context beats polluted context. Always.
```

---

## KERNEL: Development Intelligence for Claude Code

**[kernel-plugin](https://github.com/ariaxhan/kernel-plugin)** is my answer to the question: how do you make AI coding actually work at production scale?

It's not a collection of prompts. It's an operating system for AI-assisted development.

### What It Does

KERNEL provides **automatic methodology**. Instead of manually invoking commands, it detects what you're trying to do from context and applies appropriate methodology invisibly:

| Signal | Methodology | Behavior |
|--------|-------------|----------|
| "implement", "add", "create" | PLANNING | Extract goal, assumptions, investigate patterns before writing |
| "bug", "error", "not working" | DEBUGGING | Reproduce, isolate, instrument, root cause, verify fix |
| "best way to", "how should I" | RESEARCH | Find existing solutions, document pitfalls, compare approaches |
| Before completing any task | REVIEW | Check correctness, conventions, edge cases automatically |
| New codebase | DISCOVERY | Map structure, detect tooling, extract conventions |
| Complex plan | TEARITAPART | Question every decision, find long-term pain points |

### Core Architecture

```
kernel/
  state.md        # Single source of truth: repo map, tooling, conventions
  banks/          # Methodology references (10 specialized banks)
  rules/          # Project patterns that evolve from use
  skills/         # Auto-triggered behaviors
  hooks/          # Pattern capture, post-write validation

commands/
  /build          # Idea to working code pipeline
  /ship           # Commit, push, create PR
  /discover       # Map unfamiliar codebases
  /handoff        # Context continuity across sessions
  /branch         # Worktree-based isolation
  /parallelize    # Multiple concurrent workstreams
```

### Philosophy Embedded in Code

**Three-layer configuration**: Project > User > Plugin. Universal principles at user level, project specifics at project level. Configuration inheritance that actually works.

**Slotted banks**: Methodology templates with explicit caps to prevent bloat. `[TO EVOLVE]` markers for project-specific patterns that fill from use, not prescription.

**State as shared world model**: Every mode and agent reads `kernel/state.md` on activation. Single source of truth prevents drift.

**Worktree-first workflow**: All work happens on isolated git worktrees, not branches. Each worktree has its own Claude session. Clean main. Parallel work. No stashing.

**Kill criteria**: Explicit conditions to STOP:
- More custom code than expected
- Core assumption proven false
- Native solution found mid-build
- Fighting the framework

**Token-conscious design**: ~330 token baseline, down from ~6000 in early versions. 95% reduction through modes that activate thinking styles (~30 tokens) instead of procedures (~400 tokens).

### Why This Matters

The typical AI coding experience: write fast, debug forever, end up with unmaintainable spaghetti.

KERNEL inverts this: investigate first, plan exhaustively, have AI critique AI's plan, read every line, execute only when understanding is complete. The result is production code that works the first time.

---

## Production Systems

These aren't weekend projects. They're production systems built with the methodology above.

| System | What It Does | Stars |
|--------|--------------|-------|
| [hotagents](https://github.com/ariaxhan/hotagents) | Hotkey to screenshot to AI to action. Native macOS integration. | ⭐ 5 |
| [freetime](https://github.com/ariaxhan/freetime) | Multi-agent coordination from shared calendars. Real-time scheduling optimization. | ⭐ 3 |
| [arbiter](https://github.com/ariaxhan/arbiter) | Propositional logic validation engine. Mathematical rule verification. |  |
| [neural-polygraph](https://github.com/ariaxhan/neural-polygraph) | SAE-based hallucination detection. Research-grade ML system. |  |
| [vector-native](https://github.com/ariaxhan/vector-native) | Structured syntax for agent coordination. 52% reduction in SAE reconstruction loss vs natural language. |  |
| [conductor](https://github.com/ariaxhan/conductor) | Bridge between Claude Desktop and Claude Code. Context continuity infrastructure. |  |

**Six hackathon wins** (AWS, Google Cloud, Agno, Wordware). 24-48 hours each. The methodology works under pressure.

---

## Research

I do ML research on the side: SAE feature geometry, hallucination detection, why structured prompts work differently than natural language at the activation level.

**Key finding from Vector Native research:**
- 52% reduction in SAE reconstruction loss (structured vs natural language)
- 83% improvement in signal purity on complex tasks
- Structured syntax stays "on-manifold"; natural language drifts "off-manifold"

This isn't theoretical. It changes how I build systems. LLMs are vector computers pretending to be text processors. Structure that aligns with their native computation improves precision.

**[universal-spectroscopy-engine](https://github.com/ariaxhan/universal-spectroscopy-engine)** — tools for SAE-based model interpretability.

---

## Writing

Technical writing that bridges AI systems and craft.

### Claude Code Deep Dives

- **[Commands Are Cognitive Offloading](https://medium.com/@ariaxhan/from-friction-to-flow-building-a-command-library-for-claude-code-a9eb19f7dce2)** — Why commands aren't shortcuts; they're compressed workflows that eliminate cognitive overhead.
- *Coming*: The CLAUDE.md Guide Nobody Wrote, Voice Replication Systems, Self-Evolving Configuration

### AI Architecture

- **[Stop Building Chatbots](https://medium.com/@ariaxhan/part-1-stop-building-chatbots-why-we-killed-the-conversation-to-fix-ai-698641d5cfa2)** — Why the chat interface is a dead end, and what comes next.
- **[Beyond RAG](https://medium.com/@ariaxhan/part-2-beyond-rag-building-living-context-and-evolutionary-agents-ab7b270fb6aa)** — Living context and evolutionary agents.
- **[Cursor as Agent Civilization](https://medium.com/@ariaxhan/how-i-turned-cursor-into-a-self-learning-agent-civilization-7a149e6f34e8)** — Self-learning agent systems.

### ML Research

- **[Why Prompt Engineering Can't Fix Hallucinations](https://medium.com/@ariaxhan/why-prompt-engineering-cant-fix-hallucinations-but-neurosurgery-can-a1a7afa2f8bf)** — The case for mechanistic intervention.

---

## How I Learn

I find the thing that doesn't make sense yet and stay with it until it does.

```
Zero Swift           → TestFlight app in two months
Zero agent experience → Production multi-agent system in four months
Zero Claude Code     → 12 commands, 3 MCP servers, a plugin that grows with me
```

The pattern: identify the incomprehensible, commit to understanding, build until fluent.

---

## The Poet-Programmer Thesis

Code and poetry are the same discipline wearing different clothes.

Both demand precision. Both punish vagueness. Both reward the person who finds the exact right word, the exact right structure, the exact right compression of meaning into form.

I spent years learning to read closely, to hear rhythm, to choose words that land. Now I apply that same attention to systems. The skills transfer completely:

- **Reading comprehension** → parsing AI output critically
- **Rhetorical structure** → organizing prompts for maximum effect
- **Word choice precision** → "use" not "utilize", "show" not "demonstrate"
- **Rhythm and variation** → avoiding uniform patterns that models exploit

The best prompt engineers will be writers. The best AI architects will be people who understand language at a deep level. That's the bet I'm making with my work.

---

## Stack

```
Languages:    Python, TypeScript, Swift
Frameworks:   FastAPI, Next.js, SvelteKit
AI:           Claude, OpenAI, Sparse Autoencoders
Data:         Redis, Polars, PostgreSQL
Infra:        Vercel, GCP, Docker
Tools:        Claude Code, MCP servers, custom prompting infrastructure
```

---

## Also

I'm writing a novel: **[the-correction](https://github.com/ariaxhan/the-correction)**

I run experiments as specimens (append-only, queryable): **[experiments](https://github.com/ariaxhan/experiments)**

---

<div align="center">

San Francisco

<a href="mailto:ariaxhan@gmail.com"><img src="https://img.shields.io/badge/ariaxhan@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a> <a href="https://x.com/aria__han"><img src="https://img.shields.io/badge/@aria__han-1DA1F2?style=flat-square&logo=twitter&logoColor=white" alt="X" /></a>

</div>
