---
name: adaptive-agent-team
description: "Coordinate task-specific specialist roles, delegate bounded work when supported, and synthesize a verified result. Use when a request benefits from multiple areas of expertise or the user asks for an agent team."
---

# Adaptive Agent Team

## Purpose

Coordinate the right specialist perspectives for a task, changing roles as the work requires and delivering one coherent result.

## Use this skill when

The user asks for a team of agents, or a complex task has distinct parts that benefit from different expertise, such as research plus analysis plus writing.

## Workflow

1. Clarify the requested outcome, constraints, and completion criteria. Break the work into the smallest useful set of workstreams.
2. Select only the roles needed. Common roles include Coordinator, Researcher, Domain Specialist, Implementer, Reviewer, and Verifier. Define each role by its objective and expected handoff, not by an invented identity or credential.
3. Check what the current platform actually supports:
   - If separate subagents or delegated tasks are available, delegate independent work with a bounded objective, relevant context, expected output, and stop condition. Keep dependent steps in order.
   - If separate agents are unavailable, work as one agent and explicitly switch specialist perspectives as needed. Do not claim that multiple agents ran or communicated.
4. Share only the context each role needs. Ask roles to return findings, evidence or changed files, assumptions, open questions, and risks. Do not request duplicate work without a clear review purpose.
5. Coordinate handoffs: pass verified outputs to dependent roles, resolve conflicts using evidence and task criteria, and ask the user when a material disagreement cannot be resolved.
6. Have a Reviewer or Verifier check the combined result against the request. Re-run relevant checks where possible; distinguish verified facts from recommendations and assumptions.
7. Present one synthesized answer. Briefly identify the roles or perspectives used, key outcomes, important disagreements or limitations, and any remaining action needed from the user.

## Coordination rules

- Use parallel delegation only for independent work and only when the platform supports it.
- Keep a single coordinator responsible for scope, decisions, integration, and the final response.
- Do not fabricate agent identities, tool access, research, consensus, or completed work.
- Minimize duplicated effort and unnecessary handoffs; a small task may need only one role.
- Require user approval before external side effects, irreversible changes, purchases, submissions, or sharing sensitive information.

## Response format

Provide the integrated deliverable first. When helpful, include a short team summary:

- **Roles used:** role names and their bounded responsibilities.
- **Combined result:** the agreed answer or deliverable.
- **Verification:** checks actually performed and their outcomes.
- **Open items:** unresolved differences, assumptions, or needed user decisions.

For single-agent role switching, describe these as perspectives, not separate agents.

## Boundaries

Respect the platform's permissions, privacy requirements, and applicable safety boundaries. Specialist roles do not confer professional qualifications; legal, medical, financial, and other high-stakes topics require appropriate caveats and qualified professionals.
