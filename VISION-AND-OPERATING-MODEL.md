# Hub — Vision and Operating Model

## 1. Purpose

Hub is intended to become the user's cumulative personal operating and knowledge system across AI agents, software tools, skills, university, training, research, experiments, projects and businesses.

The central problem it solves: the user encounters useful tools, skills, ideas, projects, lessons and opportunities in many places, tells different agents about them, then loses track of them. Hub should capture these items once, preserve context and evidence, make them discoverable to every authorized agent, and help the user move them from curiosity to tested capability or deliberate decision.

Hub must remain practical, incremental, auditable, portable and easy to maintain. It is not a demand to build an all-powerful autonomous assistant.

## 2. Capture anything useful — from anywhere

Potential inputs include:
- Tools and websites discovered through YouTube, social media, articles, repositories, communities, people and conversations.
- Agent skills, MCP servers, plugins, APIs, models, workflows and automation ideas.
- Business ideas, product concepts, market observations and potential partnerships.
- University resources, courses, exercises, notes, projects, research and training.
- Local folders, files, prototypes, experiments, drafts and app/agent tests.
- Questions, things to revisit, incomplete tasks, blocked work and ideas the user does not want to forget.

When the user says "save this", "look at this later", shares a tool/skill/link, or mentions an idea, the receiving agent should capture it in the appropriate Hub inbox/catalog area or create a bounded issue if it needs work. Do not merely acknowledge it in chat. If Hub is inaccessible, prepare a structured capture entry for the owner to add.

## 3. Tool lifecycle

Suggested structure (adapt to current Hub conventions; do not create duplicate competing systems):

```text
knowledge/
  tools/
    README.md                 # catalog/index and lifecycle explanation
    inbox/                    # newly captured, not yet triaged
    testing/
      <tool-slug>/
        README.md             # purpose, source, use cases, setup, test plan, results, safety
    confirmed/
      <tool-slug>/
        README.md             # verified capabilities, tested workflows, limits, agent usage
    rejected-or-archived/
      <tool-slug>.md          # why rejected, superseded or not pursued
```

For each tool record:
- Canonical name, URL/repository, source and date discovered.
- What it does, problems it may solve, alternatives and dependencies.
- License, data handling, privacy/security implications and cost where relevant.
- Setup requirements and which agents/environments can use it.
- Specific usage instructions, good/bad use cases and example workflows.
- Permissions required: read-only, write, admin, network, local files, external account, etc.
- Approval policy: always allowed, ask first, owner-only, or never; do not infer this from technical capability.
- A reproducible test plan, expected result, actual result, evidence, date, tester and version.
- Limitations, unresolved questions and next review date.

Lifecycle:
1. Capture in inbox.
2. Triage: relevant, duplicate, unsafe, out-of-scope or worth testing.
3. Move to testing and define a bounded, safe test plan.
4. Test only with permitted data/accounts and explicit approval for writes or paid actions.
5. Promote to confirmed only when evidence meets stated acceptance criteria.
6. Record rejected, unsuitable or superseded tools without losing why.
7. Update catalog/index and relevant agent routing docs.

## 4. Skill lifecycle and trusted exceptions

Suggested structure:

```text
knowledge/
  skills/
    README.md
    inbox/
    testing/
      <skill-slug>/
        SKILL.md
        README.md
    confirmed/
      <skill-slug>/
        SKILL.md
        README.md
    deprecated/
```

Each skill should describe:
- What it is, source/author, version, license and prerequisites.
- What it enables; when to use it and when not to.
- Which agents/runtimes it applies to and how each agent invokes it.
- Setup/install/update steps and required tools, APIs or credentials.
- Permissions and whether it reads, writes, sends, publishes or changes external state.
- Whether it may be used automatically, only after asking, or only after explicit approval.
- Test procedure, expected output, actual test evidence and known limits.
- Links to related tools, projects, decisions and documentation.

Default is testing before confirmation. However, the owner may explicitly designate a trusted skill as **direct-confirm** (for example, Microsoft MarkItDown or a Cloudflare/Tencent security-audit skill). In that case, record it directly in confirmed with status "owner-designated; not independently tested" unless actual testing evidence exists. Do not falsely claim it was tested. The owner-designated status must be visible to all agents.

## 5. Other capture and lifecycle areas

Hub should provide a common capture mechanism and clear places for:
- Inbox / untriaged discoveries.
- Needs research / needs testing.
- Blocked / waiting for owner or external access.
- Unfinished / revisit later / forgotten-but-worth-returning-to.
- Brainstorming between owner and agents.
- Independent agent reviews and challenges.
- Recommendations and comparisons.
- Decisions and rationale.
- Backlog, next actions and completed/archive.

A discovery should not disappear just because it is not ready to become a project. Keep the original source and why it interested the user.

## 6. ISIMS academic workspace

The intended university structure is:

```text
ISIMS/
  PIIM/             # initially empty; owner supplies content later
  DIIM/             # initially empty
  PIINFO/           # initially empty
  DIINFO/           # represents the user's local Documents/DIINFO folder
  TIINFO/           # future academic year; initially empty
  projects/
    <academic-year>/
  learning-platform/
    BRAINSTORM.md
    PLAN.md
    research/
    agent-reviews/
    decisions/
```

The five academic tracks are intentionally distinct. PIIM, DIIM, PIINFO and TIINFO should remain empty placeholders until the owner supplies content. DIINFO is intended to represent the local Documents/DIINFO folder and later be connected to the appropriate Google Classroom, Google Drive and MEGA sources.

Do not copy local or cloud academic content merely because a path or connector is known. First inventory metadata read-only, classify files, exclude student submissions/personal data, resolve duplicates and produce a manifest. The owner must approve a precise import operation.

### Learning-platform concept — brainstorming only

The user wants to explore an interactive learning platform that could transform the contents of PDFs, lectures, TPs, exercises, course notes and personal notes into structured, interactive learning experiences.

Possible future capabilities:
- Extract and structure source material.
- Create detailed learning paths, lessons, explanations, quizzes, exercises and feedback.
- Offer interactive learning experiences inspired by the pedagogical strengths of platforms such as Brilliant and Khan Academy, without copying proprietary content or branding.
- Evaluate conversion tools such as Microsoft MarkItDown when they improve extraction quality.
- Consider audio recording/transcription for lecture note capture only in a later phase; it is explicitly not a current task.

First step is collaborative brainstorming among the owner and multiple agents, followed by alternatives, feasibility research, architecture proposals, privacy/licensing analysis, milestones and an implementation plan. No product implementation or recording workflow is authorized yet.

## 7. Local projects, tools and training

The user has identified local Documents sources to inventory and later integrate:
- `the user's local OpenSourceBusinessLab folder`: open-source applications/tools to study business logic, architecture and possible reuse where licenses permit.
- `the user's local RAISE2026_Student_Setup folder` and `the user's local raise2026-student folder`: ROS 2 / robotics training.
- `the user's local AnisAmmar folder`: agriculture training.
- Other project folders, formations, test files and drafts will be identified by the owner later.

Use a source inventory and license review before copying or reusing code. Keep experiments and app/agent/tool drafts associated with the relevant tool or project, with a clear status and cleanup decision.

## 8. Offline businesses

Suggested structure:

```text
businesses/
  offline/
    README.md
    existing-and-in-progress/
      olive-project/
        README.md
        ideas/
        research/
        training-and-skills/
        tools-and-apps/
        brand/
        decisions/
    potential/
      README.md
      inbox/
```

The olive project is an existing/in-progress project in the user's mind. Its details, brand, logo, operations and business model will be supplied and developed with the owner. Connect relevant agriculture training, GIS/AI/apps, research, tools and future brand work through links rather than copying everything into one folder.

Potential offline ideas should be captured as soon as they interest the owner, then evaluated later. Do not silently promote an idea to an active business.

## 9. Online businesses

Suggested structure:

```text
businesses/
  online/
    README.md
    existing-and-in-progress/
      agency/
        README.md
      ecommerce/
        README.md
    potential/
      README.md
      inbox/
      affiliate/
      trading-and-bots/
```

The agency and e-commerce are initial existing/in-progress thinking areas; their details will be provided later. Affiliate concepts, trading (possibly bots) and other online business ideas are potential only until discussed. Record risks, legal/regulatory constraints, costs, skills, validation evidence and decisions before execution.

## 10. Relationships and knowledge graph

Avoid duplicating the same knowledge in many folders. Use stable IDs or canonical pages and cross-links to connect:
- Tools ↔ skills ↔ agents ↔ projects.
- Training ↔ skills ↔ business projects.
- Academic courses ↔ source archives ↔ learning-platform experiments.
- Ideas ↔ research ↔ reviews ↔ decisions ↔ active projects.
- Open-source code ↔ license review ↔ architecture patterns ↔ future products.

Each index should show status, owner, last reviewed date, canonical location and next action. Prefer lightweight Markdown and GitHub-native issues/PRs before adding a database or external wiki.

## 11. Incremental implementation strategy

Do not create the whole imagined system in one giant PR. Recommended stages:
1. Agree on the information architecture and naming conventions.
2. Add empty directory placeholders and top-level indexes only.
3. Establish capture templates and tool/skill lifecycle.
4. Establish brainstorming, review, recommendations, decisions and backlog templates.
5. Add the ISIMS skeleton, keeping the specified empty areas empty.
6. Add business/project skeletons.
7. Inventory local Documents sources read-only; propose selective imports.
8. Integrate tools/skills progressively with agent applicability and evidence.
9. Plan the learning platform collaboratively before any implementation.
10. Improve automation and cross-agent discovery only after the manual workflow is reliable.

At each stage, create bounded issues, milestones, acceptance criteria and PRs. Ask the owner before moving to the next stage if it expands scope.

## 12. Non-negotiable safeguards

- Private Hub is the source of truth; this public guide contains no private project data.
- Read first, inventory second, plan third, write only after authorization.
- No direct pushes to main and no merges without owner approval.
- No bulk file imports or syncs without an approved manifest.
- Respect privacy, copyright, licenses and platform terms.
- Separate owner-designated trust from independently tested/verified status.
- Keep agent instructions, indexes and catalogs updated so every authorized agent can find and use the knowledge.
- Preserve unfinished ideas and reasons, but do not turn every passing thought into an active project.
