# Capturing a Chat-Project's History into the Private Hub

Public and generic. This page describes a procedure. It contains no project or client names, no private Hub content, no paths and no credentials, and it grants no access.

## Why
Chat Projects (a Claude Project, a ChatGPT Project and similar) accumulate decisions, code reviews, test results and plans that other agents cannot see. The private Hub is the durable shared layer. Capturing a project's history there lets any authorized agent answer four questions without asking the owner to repeat themselves: what has been done, what is being built, what is being discussed, and what is still open.

## Preconditions
1. The owner asked for, or approved, the capture of that specific project and the target repository.
2. Verify your own access (read, write, which repositories). Another agent's access or credentials never apply to you.
3. If you cannot reach the private Hub, say so. Prepare the record as one fenced block for the owner to paste, and do not pretend to know private status.

## Procedure
1. Cold start: read the Hub's contract files first (AGENTS.md, STATUS.md, context.md, INDEX.md).
2. Inspect existing project records, open issues and open PRs before writing. Do not duplicate. Avoid files that other open PRs are editing (line-capped status files, shared indexes); append new sections elsewhere instead.
3. One issue, one claim, one dedicated branch, one PR. Never push to `main`, never merge. Commits carry the required `Agent:` and `Refs:` trailers. With only an API (no shell or worktree), build one trailered commit through the Git Data API and say so in the claim.
4. Create `projects/<slug>/` following the structure of existing records: a README entry point (purpose, boundaries, read order, state at a glance, records table), a charter, architecture, decisions and open questions, a backlog, a completed-work or evidence register, a timeline with sources, and a learnings file when the project produced reusable lessons.
5. Make it discoverable: add it to the projects catalog and link from related areas. If two things share a name (for example an academic project and a client project), add a disambiguation note on both sides and do not assert a relationship you cannot verify.
6. Cross-check conversation claims against the real artifacts (code repository, deployed endpoints) read-only. Record what the check found, including problems the conversation never mentioned.
7. Check relative links and scan for secrets and personal data before committing. Post EVIDENCE and HANDOFF on the issue, then stop for owner review.

## Evidence labels
- **verified**: checked now, with a link or command.
- **observed**: seen earlier and dated; re-test before relying on it.
- **reported**: stated in the conversation or a memory summary; not re-checked.
- **owner direction**, **proposed**, **unknown**.

A recommendation made in chat is *proposed*, not done. A tool that was mentioned is not installed. If only a memory summary is available (no transcripts), say so and mark dates and links as not recovered rather than inventing them.

## What never goes in
Secrets, tokens, webhook or deployment URLs that act as credentials, absolute home paths, personal or client data (contact details, form submissions, leads, CVs), raw source files, bulk copyrighted material. For client or freelance work, record only architecture, decisions, status, evidence and pointers to the code repository. When you notice something sensitive (for example an address inside a public repository), record *that* it exists and where to look, never the value.

## Field notes from real delivery work
Observed on one web project. Generic, but re-verify for yours.
- Do not load-test production endpoints that have side effects (email, spreadsheet writes, payments). Test a duplicate deployment pointing at test data.
- Bursts from a single IP against a CDN-fronted site trigger rate limiting, so the numbers describe bot protection, not capacity. Use staged ramp-up with think time and realistic multi-page journeys.
- Serverless script web apps (for example Apps Script) serve the deployed version. Saving edits is not enough; publish a new deployment version.
- Some MCP tools time out on long processes (observed around 40 seconds). Start the process, keep its ID, poll for output.
- Some edit tools fail on the local filesystem through MCP; rewriting the whole file with the write tool worked.
- Cloud-synced folders plus framework build caches can cause dev-server crash loops. Clear the cache or keep projects outside synced folders.
- When several AI-generated variants of one project exist, choose by deployment-readiness evidence (config, working functions, real build output), then port specific parts.
- Review config flags that silence checks (for example ignoring build type errors) before adding features.
