---
name: pr-metadata-placement
description: Place lasting project information in repository records, PR-specific coordination in pull request metadata, and CI check outcomes in CI run records. Use when writing, updating, or reviewing repository documentation, pull request descriptions, or pull request comments.
---

# PR Metadata Placement

Use this skill when writing, updating, or reviewing repository documentation, pull request descriptions, or pull request comments, including text about CI test results and check status.

## Core rule

Keep information that defines the project or its outstanding obligations in the established repository canon. Keep information about a particular pull request's coordination and lifecycle in that pull request. Keep the execution state and conclusions of CI checks in their owning CI run records.

Choose the record according to the information's responsibility:

- **Repository canon:** accepted requirements and design, implementation and test plans, durable task-to-task dependencies, required verification and reproducible work evidence, standing workflow rules (including CI acceptance criteria), and project work tracked by an established handoff process.
- **CI runs and checks:** execution status, individual job conclusions, diagnostic logs, and rerun outcomes for the checked commit.
- **PR body:** references to other PRs, prerequisite merges, intended integration order, current review or merge waits, active blockers, and the current coordination status of that PR, with links to CI checks when relevant.
- **PR comments:** dated progress, status transitions, review discussion, and coordination history. Maintain the current status summary in the PR body.

Record a cross-PR prerequisite in the body of the PR that depends on it. Link the prerequisite PR and describe the condition for proceeding.

## Apply during writing and review

1. Determine whether each statement describes a durable project fact or obligation, the outcome of a particular CI execution, or coordination for a specific PR.
2. Put project decisions, required checks, reproducible verification facts, and outstanding work in their canonical records; use the owning CI checks for run-specific pass/fail and the affected PR for coordination.
3. When repository prose ties an implementation or completion claim to a particular CI check result, express the lasting project fact or required evidence independently of that result. Move run-specific outcomes and current check state to the owning CI run or linked PR.
4. When PR-specific coordination appears in a repository document, transfer that coordination to the relevant PR while preserving independently relevant project facts in the canon.
5. Update the PR body when a coordination condition changes; use comments for the progression and discussion when useful.
6. During review, verify that repository prose remains true independently of CI reruns or changes to the checked commit, and that changed records follow the same placement boundary.

For example, an implementation handoff obligation recorded by a design workflow belongs in the design canon even while outstanding. A wait for another PR to merge belongs in the waiting PR's body.

## Responsibility boundary

This skill determines where information is recorded. CI run records retain results and logs; the existing requirements, design, planning, review, branching, and merge workflows determine the underlying obligations and acceptance conditions.

This skill targets repositories maintained by a single user working with an AI agent.
