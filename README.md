# Tronijess

**Tronijess = Tron + Jess.** A reversal of Jessitron (human augmented by code), Tronijess is code that works like humans do.

I'm Jessitron, and this is my personal agent system - but it's also a learning laboratory for understanding how agents collaborate, how they should be developed, and how to make them radically observable.

## Why This Exists

I'm building this to explore three questions:

- 🧑‍🤝‍🧑 **How do agents work together?** Not just one AI doing tasks, but a consulting firm of specialized agents collaborating
- 🔭 **How do we make agent systems observable?** Not just logs, but true transparency into reasoning and decision-making
- 🔁 **What makes a codebase agent-friendly?** How might projects be structured when agents are the primary developers?

Also, I really want a personal agent 💕

### Tronijess helps me with:

- **Executive assistance** - Keeping track of what I'm working on, helping me with executive function, someday carrying out tasks for me
- **Coding** - Building software with agent assistance, just like hiring a crack software shop to build and steward my precious projects
- **Learning** - Recording and organizing what I discover, both here and in the world.

## What Makes This Interesting

- **Agents as Bounded Contexts:** Each agent owns a domain (eg, in a coding project: tasks, code, learning) with its own knowledge base, versioned in git. They communicate across boundaries like microservices - by asking questions, not sharing databases.
- **Retroactive Introspection:** Because agent contexts can be perfectly reconstructed from git history, we can do something impossible with humans: go back to any point and ask "what were you thinking here?" This isn't logging reasoning at the time - it's lazy evaluation of introspection.
- **Observable by Design:** Every agent interaction is traced with commit SHAs. We can see not just what happened, but reconstruct the complete context at any decision point. The whole system is built for transparency.
- **Code That Works Like Humans:** Agents have specialties (PM, architect, librarian, bard), they collaborate through conversation, and they maintain their own knowledge domains. But they never context-switch - we just spawn multiple conversations. And they have perfect recall through git.

## What It Does

Each coding project gets its own team of agents, all working in the same repo with separate domain directories.

The executive assistant gets its own repo, and might create new projects and "hire" the consulting firm to work on them.

The personal librarian will someday update and run a wiki ☺️

### The Bootstrap

This project is being built by agents (Claude Code initially, then Tronijess itself). We're practicing what we're building - using domain separation, capturing decisions, and making everything observable from day one.

The project structure mirrors the coding-agent architecture:

- `domain-tasks/` - Project management and task tracking
- `domain-code/` - Code and technical artifacts
- `domain-learning/` - Documentation, decisions, and knowledge

Each domain has its own agent prompt defining the role, boundaries, and responsibilities.

## What I'm Learning

This is as much about the journey as the destination. The `domain-learning/` directory captures the evolving understanding of how to build agent systems that are transparent, collaborative, and maintainable.
