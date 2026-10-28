# pr-metadata-placement

A lightweight skill for placing persistent project information in repository records and PR-specific coordination in pull request metadata. Designed for a single-user AI-agent repository workflow.

## When to use

Use when writing, updating, or reviewing repository documentation, pull request descriptions, or pull request comments.

## Core idea

Keep accepted requirements, design, plans, and project obligations in their established canonical repository documents. Keep prerequisite PR links, merge waits, review status, and other PR-specific coordination in the affected PR's body. Use comments for progress and coordination history.

This keeps repository documents focused on the state of the project while PRs carry the transient state of integrating their changes.

Existing requirements, design, planning, review, branching, and merge workflows own the underlying decisions; this skill owns the placement of their records.

## Installation

Install this repository as a skill folder in an AI-agent environment that supports SKILL.md-based skills. Keep SKILL.md at the skill folder root and register or reference it from the repository's relevant documentation, pull-request, and review work-type entry points.

## Files

- SKILL.md — installable skill definition and placement procedure.
- README.md — usage and installation guidance.
- LICENSE — MIT License.
