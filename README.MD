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

**[kernel-plugin](https://github.com/ariaxhan/kernel-plugin)** | v2.0.0

Run `/kernel-init` and KERNEL analyzes your codebase, then generates a complete custom configuration: commands for your workflows, agents for your stack, rules from your patterns, skills for repeated tasks. Everything you don't want to set up yourself.

### What It Does

**Generates custom config per project.** Not templates. Tailored artifacts based on what KERNEL finds in your codebase:

- `.claude/CLAUDE.md` — Project-specific coding rules
- `.claude/commands/` — Workflows for your stack (test commands, deploy scripts)
- `.claude/agents/` — Specialized agents (test-runner if you have pytest, type-checker if you have TypeScript)
- `.claude/rules/` — Patterns discovered in your code
- `_meta/` — Session tracking structure

**Methodology applies automatically.** Once initialized, KERNEL detects what you're doing:

| You're doing... | KERNEL automatically... |
|-----------------|-------------------------|
| Implementing new feature | Researches, plans, defines interfaces first |
| Fixing a bug | Reproduces, isolates, finds root cause |
| Refactoring | Understands deeply before changing |
| Writing code | Spawns test-runner, type-checker |
| Completing work | Reviews against requirements |

**Proactive agents.** 13 specialized agents spawn based on context:

| Fast Validation (Haiku) | Deep Analysis (Opus) |
|-------------------------|----------------------|
| test-runner, type-checker | code-reviewer, security-scanner |
| lint-fixer, build-validator | test-generator, api-documenter |
| dependency-auditor, git-historian | perf-profiler, refactor-scout |
| **git-sync**, **metadata-sync** | debugger-deep, database-architect |

`git-sync` and `metadata-sync` run at end of every response. Auto-commit. Auto-push. Auto-update session state.

**Session continuity.** The `_meta/` structure tracks context across conversations:

```
_meta/
├── INDEX.md              # Navigation hub
├── _session.md           # Session context (blockers, decisions)
├── _learnings.md         # Change log (append-only)
├── context/
│   └── active.md         # Current work state
└── research/
    └── *.md              # Investigation outputs
```

### Architecture

```
kernel-plugin/
├── _meta/                 # Session tracking (v2.0.0)
├── commands/              # 14 commands
│   ├── /build             # Idea → research → plan → implement → validate
│   ├── /ship              # Commit, push, create PR
│   ├── /validate          # Pre-commit gate: types + lint + tests
│   ├── /iterate           # Continuous improvement
│   ├── /tearitapart       # Critical review before implementing
│   └── ...
├── kernel/
│   ├── agents/            # 13 specialized agents
│   ├── skills/            # 3 auto-triggered capabilities
│   ├── banks/             # 10 methodology templates
│   ├── rules/             # 11 foundational constraints
│   └── state.md           # Project reality tracker
```

**14 commands. 13 agents. 10 banks. 11 rules. 3 skills.**

### Philosophy

**Self-evolution.** When patterns emerge, KERNEL captures them:
```
Learn → Log to _meta/_learnings.md → Update configs → Commit & push
```
Patterns compound. Mistakes don't repeat.

**Tailored, not templated.** Every artifact exists because your project needs it. Not because a template includes it.

**Token-conscious.** ~200 token baseline (vs ~6000+ traditional). Banks load on-demand. Agents spawn only when relevant.

---

## Projects

| Project | What It Does |
|---------|--------------|
| [hotagents](https://github.com/ariaxhan/hotagents) | Hotkey → screenshot → AI → action |
| [freetime](https://github.com/ariaxhan/freetime) | Multi-agent coordination from shared calendars |
| [arbiter](https://github.com/ariaxhan/arbiter) | Propositional logic validation engine |
| [neural-polygraph](https://github.com/ariaxhan/neural-polygraph) | SAE-based hallucination detection |
| [vector-native](https://github.com/ariaxhan/vector-native) | Structured syntax for agent coordination |
| [conductor](https://github.com/ariaxhan/conductor) | Bridge between Claude Desktop and Claude Code |

**Six hackathon wins** (AWS, Google Cloud, Agno, Wordware). 24-48 hours each.

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
