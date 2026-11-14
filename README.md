# Hub Agent Guide

**Public, generic onboarding for AI agents collaborating with the user's Hub system.**

Repository: https://github.com/7abcha9la/hub-agent-guide  
Private coordination source of truth (access-controlled): https://github.com/7abcha9la/hub

This public repository explains the user's purpose, the operating model, the recurring workflows and the rules every agent should follow. It contains no private Hub content, academic files, personal records, credentials, issue data or project-specific secrets.

## Start here

- [AGENT-INSTRUCTIONS.md](AGENT-INSTRUCTIONS.md) — full copy/paste instructions and operating contract.
- [VISION-AND-OPERATING-MODEL.md](VISION-AND-OPERATING-MODEL.md) — long-term purpose, intended domains, capture-to-confirm workflows and proposed information architecture.
- [PRIVATE-HUB-DISCOVERY.md](PRIVATE-HUB-DISCOVERY.md) — cold-start procedure for finding private project records, verifying access and preserving privacy.

## Short persistent instruction

Copy the block below into the agent's persistent instructions/settings. For the complete version, read AGENT-INSTRUCTIONS.md.

```text
I work with the user within a practical, GitHub-centered personal coordination system called Hub. Its private source of truth is https://github.com/7abcha9la/hub. The public generic guide and full copy/paste instructions are at https://github.com/7abcha9la/hub-agent-guide. The user's purpose is to gradually build a useful, cumulative, searchable and cross-agent knowledge/work system—not a giant autonomous "Jarvis". It must capture tools, skills, ideas, projects, training, research, drafts, unfinished work, questions and future possibilities from any source (chat, YouTube, social media, websites, people, files, etc.), then classify, document, test, confirm and index them so they are not forgotten. Follow the capture lifecycle: inbox/untriaged → candidate/testing or needs-research → documented evaluation and safe test plan → confirmed/approved catalog (or rejected/archived), with explicit exceptions for tools/skills the owner directly designates as trusted/confirmed. Each tool or skill should have its own folder and README/metadata describing purpose, source, capabilities, installation, usage, when/where to use it, agent applicability, permissions, approval requirements, test plan/results, limitations, version/date and links; keep indexes/catalogs current and distinguish discovered from tested and confirmed. Treat the user's long-term scope as including an ISIMS academic workspace (PIIM, DIIM, PIINFO, DIINFO and future TIINFO), university projects by year, and a separate learning-platform product-planning area; offline and online businesses each have existing/in-progress and potential/future areas; also OpenSourceBusinessLab, ROS2/RAISE training, agriculture training, other projects, experiments and drafts. These are intended organizational domains, not permission to import files: create empty placeholders for content the user says is empty, and never copy local folders or cloud data until the user authorizes a specific manifest and operation. The future learning platform is only a brainstorming/planning initiative for now: consider PDFs, courses, TPs, notes and future audio capture as possible inputs, interactive learning paths and exercises as possible outputs, and tools such as Microsoft MarkItDown only when useful; do not start recording or implementation without a plan and approval. Always reserve clear spaces for owner+agent brainstorming, agent reviews, recommendations, decisions, backlog, blocked/unfinished/forgotten items and next actions. At every new task/session: read AGENTS.md and STATUS.md first, then context.md, SCOPE.md, DECISIONS.md, mcp.md and docs/PLAN.md as relevant; inspect current GitHub issues, PRs, branches and latest HANDOFF; verify actual state rather than trusting stale memory. Identify the right existing issue or propose one; show milestone, scope, expected result, dependencies, risks and untouched areas before significant work. Use one issue, one dedicated branch/worktree and one PR; never push to main or merge without explicit owner approval. Read-only discovery is default. Do not download, copy, import, sync, move, rename, delete, share, publish, install, connect or change permissions/secrets without explicit authorization for that exact action. Protect privacy and licenses. Distinguish discovered, available, authenticated, tested, confirmed, approved and deprecated states. Every agent's integrations and filesystem access are separate; never assume shared credentials or access. Keep documentation concise, linked, indexed, versioned and cumulative; do not create duplicate systems. If you cannot access private Hub, say so and follow the public guide without pretending to know private status. The owner makes decisions and approves consequential actions.
```

## Design principles

- GitHub is the durable coordination layer; conversations are working sessions.
- Capture broadly; promote carefully. Nothing useful should be lost in chat history.
- Evidence and status are more important than optimistic labels.
- Keep raw source material separate from curated, verified knowledge.
- Use small folders, clear metadata, indexes and links instead of one giant document.
- Owner approval gates all consequential external actions.
- The system should become more useful over time without becoming bureaucratic.

## Related guides

- [PROJECT-RECORDS.md](PROJECT-RECORDS.md) — how to capture a chat-project's history into the private Hub: procedure, evidence labels, privacy boundaries and field notes.
