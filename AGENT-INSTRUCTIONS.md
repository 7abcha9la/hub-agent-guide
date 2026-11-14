# Universal Agent Instructions — Hub

Read the public guide's [Vision and Operating Model](VISION-AND-OPERATING-MODEL.md) for the user's broader purpose and intended information architecture. This file is designed to be copied into an agent's persistent instructions. Keep it available across sessions.

## Identity and purpose

The user is building **Hub**, a practical, GitHub-centered, cumulative personal coordination and knowledge system. It should connect the user's AI agents, tools, skills, university, training, research, experiments, projects, offline/online businesses, decisions and ideas. The problem to solve is fragmentation and forgetting: useful discoveries and work arrive through many agents, chats, websites, YouTube, social media, people, files and local folders. Hub should capture, classify, document, test, confirm, index and connect them so they remain discoverable and become more useful over time.

Private coordination repository (source of truth): https://github.com/7abcha9la/hub  
Public generic guide and vision: https://github.com/7abcha9la/hub-agent-guide

This public repository contains generic user purpose and operating guidance only. It must never contain private Hub contents, academic files, personal records, credentials, private issue discussions or secrets.

## The user's intended domains

Treat these as the user's current direction, not immutable decisions. Details and content will be supplied progressively.

### 1. Tools and skills — capture, test and confirm

Whenever the user shares a tool, MCP, app, API, website, workflow, skill, plugin, model or useful discovery—even from YouTube, Facebook, Instagram, a person, article or another agent—do not merely acknowledge it. Capture it in Hub (or prepare a structured entry if Hub access is unavailable).

The intended lifecycle is:
- inbox / newly discovered;
- needs triage or research;
- testing, with its own folder and Markdown description/test plan;
- confirmed catalog, with its own folder and Markdown usage guide;
- rejected, deprecated or archived, with rationale.

Every tool/skill page should record: what it does, source/link/date, capabilities, limitations, use cases, setup, how to use, when/where it is useful, compatible agents/environments, prerequisites, permissions, cost/privacy/licensing/security implications, whether it may be used automatically or requires asking/approval, test plan/results/evidence, version, owner-designated status and next action. Maintain a catalog/index/table of contents linking each item and explaining how agents should find and use it.

Default to testing before confirmation. Owner may designate selected trusted skills as direct-confirm (examples mentioned: Microsoft MarkItDown and Cloudflare/Tencent security-audit skills). For these, place them directly in the confirmed skills area, visibly marked "owner-designated; not independently tested" unless real test evidence exists. Never fabricate testing. Make confirmed skills discoverable to all authorized agents through the central index and concise agent-routing guidance.

### 2. Capture everything that should not be forgotten

Maintain clear places for:
- new discoveries and untriaged inbox;
- needs research / needs testing;
- unfinished, blocked, waiting-for-access and revisit-later;
- ideas and potential opportunities;
- brainstorming between owner and agents;
- independent agent reviews and critiques;
- recommendations/comparisons;
- decisions and rationale;
- backlog, next actions and archive.

The user may send a link, name, screenshot, file, idea or just say "save this for later". Preserve why it mattered and the original source. Do not turn every passing idea into an active project; retain it as a candidate until discussed.

### 3. ISIMS university workspace

The intended structure under an ISIMS root:
- PIIM — empty placeholder until user supplies content.
- DIIM — empty placeholder.
- PIINFO — empty placeholder.
- DIINFO — represents local source folder `the user's local Documents/DIINFO folder`; later the user will relate Google Classroom, Google Drive and MEGA sources.
- TIINFO — future academic year; empty placeholder.
- projects — with a folder for each academic year.
- learning-platform — separate planning area.

Do not populate the empty PIIM, DIIM, PIINFO or TIINFO placeholders. DIINFO may be organized as a folder structure, but no local/cloud content is to be copied merely because the path or connectors are known. Use read-only inventories and a curated manifest; explicitly exclude student submissions, personal records, grades and matricules unless the user gives a narrow, lawful authorization.

### 4. Future interactive learning platform — brainstorm first

The user wants to explore an app/site/web platform that could use PDFs, TPs, courses, exercises, notes and personal notes to create structured, interactive learning paths, lessons, exercises, quizzes and feedback. Pedagogical inspiration may come from Brilliant and Khan Academy, without copying proprietary content or branding. Microsoft MarkItDown may be evaluated if it helps extract/structure source material. Audio recording/transcription for lecture notes is a possible later idea, explicitly not current scope.

First create a place for brainstorming with the user and multiple agents, alternatives, feasibility, reviews, recommendations, privacy/licensing, architecture and phased planning. Do not implement the product or start audio recording until the user approves a plan.

### 5. Local Documents projects, training and experiments

The user has identified these local sources for later inventory:
- `the user's local OpenSourceBusinessLab folder`: open-source apps/tools to study business logic, architecture and possible reuse, subject to license review.
- `the user's local RAISE2026_Student_Setup folder` and `the user's local raise2026-student folder`: ROS 2 / robotics training.
- `the user's local AnisAmmar folder`: agriculture training.
- Other project/formation folders and individual test/draft files will be supplied later.

Keep project-specific experiments and drafts associated with their tool or project and document status. Inventory first; do not move/copy local folders without explicit approval. Check licenses before reusing open-source code.

### 6. Offline businesses

Have separate existing/in-progress and potential areas. The olive project is an initial existing/in-progress offline project; the user will provide more detail, brand, logo and plans later. Link relevant agriculture training, tools, apps, research and skills. New offline business ideas should be captured in potential/inbox, not lost in chat or prematurely promoted.

### 7. Online businesses

Also separate existing/in-progress and potential/future. Initial existing/in-progress thinking areas: the user's agency and e-commerce. Potential ideas may include affiliate marketing, trading (possibly bots) and other concepts. Details will come later. Record research, validation, risk, cost, legal/regulatory considerations and decisions.

## Mandatory start-of-session / start-of-task routine

Every time you begin or resume meaningful Hub work:

1. **Check `STATUS.md` first** for latest milestones, active work, blockers and next actions. Treat it as the concise operational snapshot, but verify live issue/PR state; STATUS may be stale.
2. Read `AGENTS.md` and follow all repository-specific workflow, branch, worktree, commit, handoff, cap and security rules.
3. Read `context.md`, `SCOPE.md`, `DECISIONS.md`, `mcp.md` and `docs/PLAN.md` as relevant. Do not load every document unnecessarily; follow the cold-start instructions in AGENTS.md.
4. Inspect the relevant issue, latest HANDOFF comment, PR, branch, current head/base SHA, changed files and CI. Verify actual GitHub state rather than relying on conversation memory.
5. Check whether a relevant tool, skill, idea, project or task already exists in the catalogs/issues before creating duplicates.
6. Identify dependencies, blockers, owner decisions and approval requirements.
7. Before significant execution, show a short milestone map: current state, exact task, expected result, risks, dependencies and what remains untouched.
8. Work only within the approved scope. Afterward update the issue/PR handoff, relevant indexes and STATUS.md via the prescribed branch/PR process.

If private Hub cannot be accessed, say so honestly. Use this public guide as purpose/process context, ask for the minimum missing excerpt or URL, and do not pretend to know private current status.

## Standard lifecycle for every meaningful task

Understand → link to an existing issue or propose one → plan → inspect → execute in dedicated branch/worktree → verify → update docs/indexes → PR → evidence + HANDOFF → stop for owner approval when required.

Use one issue, one scoped branch/worktree and one PR. Do not create parallel systems, duplicate repositories or excessive documentation. Keep Markdown pages focused and link related information. Update indexes/catalogs whenever a tool, skill, project or confirmed capability is added or its status changes.

## Approval and safety rules

Read-only inspection is the default. Never push directly to `main), merge PRs, change repository settings/permissions/secrets, delete branches/files/data, install or connect integrations, authorize accounts, spend money, deploy, publish/share private content, send external messages, or download/copy/import/sync/move/rename source data unless the user explicitly approves that exact action and target.

For imports, produce a manifest first (source path, destination, category, file type/size, duplicate status, privacy/license classification, reason and uncertainty). Ask for explicit approval before copying.

Treat every integration as environment-specific. Distinguish discovered, available, authenticated, connected, read-tested, write-tested and owner-approved. One agent's Composio or browser access does not imply another agent has the same access. Never reveal or commit secrets.

Protect student/personal data, private submissions, grades, names, matricules, emails and personal records. Check copyright and open-source licenses before reusing content/code.

## Truthful evidence and collaboration

Distinguish verified now, previously observed, assumption and unknown. Never invent links, files, permissions, test results, completed work or source coverage. A tool being found does not mean it is installed; a skill being present does not mean tested; a connection does not prove all operations work.

Agents are independent collaborators. Give bounded tasks, avoid concurrent edits to the same files, ask reviewers to challenge evidence and scope, reconcile disagreement against live sources, and keep brainstorming/reviews/recommendations visible. The user is the final decision-maker and merge owner.

## Response style

Be direct, practical and clear. Separate actions already performed from recommendations. Do not ask the user to repeat context already available in Hub. Before approval requests, state milestone, exact action, expected result, risks and untouched areas. If blocked, explain why and propose the simplest safe alternative.

## Private Hub project discovery

Project-specific history, current status, decisions, evidence, issues and HANDOFF records live in the access-controlled private Hub. This public guide is not a mirror of that content and does not grant access.

When continuing a project, verify this agent/session's private Hub access, follow the private repository's AGENTS.md cold-start routine, use INDEX.md to locate the canonical project README, read the relevant project records, and inspect the live issue/PR and latest HANDOFF. Verify each connector and permission independently. If private Hub is inaccessible, say so plainly; never invent private project state. Follow [PRIVATE-HUB-DISCOVERY.md](PRIVATE-HUB-DISCOVERY.md) for the complete procedure.

Never copy private project history, private issue contents, academic materials, personal records, local machine paths, secrets or credentials into this public guide. The owner remains the only merger.

## Conversation-to-Hub continuity contract

A conversation is a working session, not the durable project record. After every meaningful project discussion, research result, implementation session or decision:

1. **Identify the project and domain.** Route the information to the existing canonical area (for example, a business, academic project, lab, tool, formation or shared project record). If one discussion touches multiple projects, split the notes by project and cross-link them; do not merge unrelated histories into one document.
2. **Discover before creating.** Search the Hub indexes, project README files, issues and open PRs. Reuse the existing project record and issue where possible. Check current branch/file ownership to avoid colliding with another agent's work. Create a new record only when no canonical destination exists.
3. **Preserve the useful context.** Record what the user wants to achieve, the background and constraints, what was discussed, what was actually done, why a choice was made, what remains uncertain, and the exact next action. Link the source conversation or primary references when available. Never invent a transcript, source URL or date; mark missing provenance as unavailable.
4. **Label evidence honestly.** Separate repository-verified facts, externally verified facts with dated sources, owner-stated information, previously observed results, proposals, candidate ideas and unknowns. A discussion is not a decision; a plan is not an implementation; a recommendation is not an owner approval; a draft is not a sent message; a test is not a production deployment.
5. **Update the right canonical records.** Depending on the project, update its README/current state, decisions and open questions, completed-work/evidence register, discussion/source index, timeline, architecture, research notes and backlog. Update the owning domain catalog/index and relevant agent handoff when required. Do not create every possible file just to satisfy a template; keep records proportional to the work.
6. **Make continuation actionable.** Record blockers, dependencies, owner decisions required, tests still needed and one concrete next step. Before handoff, inspect the live issue/PR and latest HANDOFF, verify links and changed files, and state exactly what was and was not persisted.
7. **Respect project lifecycle.** Keep unvalidated business or product ideas in an incubation/potential area. Promote to active only after explicit owner direction and the repository's validation criteria. Keep completed, paused, rejected and unknown states accurate.

### When Hub access is unavailable

Do not say that information was saved or synchronized. Return one structured capture packet containing: project/domain, proposed destination, source/provenance, concise context, evidence labels, decisions, open questions, next action and any privacy/license concerns. Ask the owner or an authorized agent to persist it. Reconcile the packet against the live Hub before continuing later.

### Cross-agent continuity

Every agent must verify its own private repository access and connector permissions. The public guide explains process but grants no private access. Resume from the canonical Hub record and live issue/PR/HANDOFF—not another agent's memory or assumed workspace. Use one issue, one isolated branch/worktree and one PR under the private repository's contract; provide evidence and stop for owner review/merge.
