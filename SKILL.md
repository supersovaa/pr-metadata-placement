---
name: pr-metadata-placement
description: Place lasting project information in repository records and PR-specific coordination in pull request metadata. Use when writing, updating, or reviewing repository documentation, pull request descriptions, or pull request comments.
---

# PR Metadata Placement

Use this skill when writing, updating, or reviewing repository documentation, pull request descriptions, or pull request comments.

## Core rule

Keep information that defines the project or its outstanding obligations in the established repository canon. Keep information about a particular pull request's coordination and lifecycle in that pull request.

Choose the record according to the information's responsibility:

- **Repository canon:** accepted requirements and design, implementation and test plans, durable task-to-task dependencies, required verification evidence, standing workflow rules, and project work tracked by an established handoff process.
- **PR body:** references to other PRs, prerequisite merges, intended integration order, current review or merge waits, active blockers, and the current coordination status of that PR.
- **PR comments:** dated progress, status transitions, review discussion, and coordination history. Maintain the current status summary in the PR body.

Record a cross-PR prerequisite in the body of the PR that depends on it. Link the prerequisite PR and describe the condition for proceeding.

## Apply during writing and review

1. Determine whether each statement describes the project deliverable or coordination for a specific PR.
2. Put project decisions and outstanding work in their canonical records; put PR-specific coordination in the affected PR body or comments.
3. When PR-specific coordination appears in a repository document, transfer that coordination to the relevant PR while preserving independently relevant project facts in the canon.
4. Update the PR body when a coordination condition changes; use comments for the progression and discussion when useful.
5. During review, verify that changed records follow the same placement boundary.

For example, an implementation handoff obligation recorded by a design workflow belongs in the design canon even while outstanding. A wait for another PR to merge belongs in the waiting PR's body.

## Responsibility boundary

This skill determines where information is recorded. The existing requirements, design, planning, review, branching, and merge workflows determine the underlying obligations and acceptance conditions.

This skill targets repositories maintained by a single user working with an AI agent.
