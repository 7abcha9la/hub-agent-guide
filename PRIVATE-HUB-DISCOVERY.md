# Private Hub Project Discovery

This guide is public and generic. Project-specific records, current status, decisions, evidence, private discussions and task handoffs live in the access-controlled private Hub repository:

https://github.com/7abcha9la/hub

## Cold-start procedure

When the user asks you to continue work on a Hub project:

1. **Verify access.** Confirm that this agent/session can actually read the private repository. A public guide link or another agent's access is not proof.
2. **Read the operating contract.** In the private Hub, read AGENTS.md, STATUS.md and context.md, then follow the cold-start instructions in AGENTS.md.
3. **Find the project.** Use INDEX.md to locate its canonical project README. Do not guess paths or create a duplicate project record.
4. **Read the project entry points.** Read the project README and the relevant charter, architecture, status, decisions, backlog and source index.
5. **Inspect live work.** Check the linked GitHub issue, latest HANDOFF, open PR, branch and CI. Verify live state rather than trusting a summary.
6. **Check permissions independently.** Verify this agent's own GitHub, app, connector, MCP and filesystem access before using it.
7. **Resume within scope.** Use the existing issue where possible. Otherwise propose a bounded issue before significant work. Follow one issue = one branch = one PR.
8. **Record the outcome.** Update evidence, decisions, status, indexes and HANDOFF through the approved branch/PR workflow.

## If private Hub is inaccessible

Say plainly that private Hub access is unavailable in this session. Do not pretend to know its project inventory, latest status, private issues or decisions. Ask the owner to connect an authorized GitHub integration or provide the minimum relevant project entry point. You may still explain this public operating guide, but do not fabricate private context.

## Access and privacy rules

- Access is per agent, account and session. Never assume another agent's OAuth connection, GitHub permissions, Composio member access, local files or credentials are shared with you.
- The public guide does not grant access to the private Hub.
- Never copy private project history, issue discussions, academic material, personal records, local machine paths, secrets or credentials into this public repository.
- Do not download, import, sync, move, delete, publish or share source data without explicit approval for the exact operation.
- Do not push directly to main or merge a PR. The owner is the merger.
- Distinguish verified, previously observed, proposed and unknown information.

## Expected handoff

Every meaningful task should leave:
- the canonical project and issue link;
- branch and PR link;
- concise evidence and verification results;
- decisions made versus recommendations;
- failures, blockers and unresolved questions;
- exact next action and intended agent.

The objective is that an authorized agent can continue without making the owner repeat context, while private project knowledge remains private.
