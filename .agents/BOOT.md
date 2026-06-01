# First-Time Setup

If this file exists, this repository is a fresh clone and must be bootstrapped before normal project work begins.

## Required Checks

Before modifying project files, inspect the available user-provided context:

- `.samples/docs/`

  - PRDs
  - requirements
  - implementation notes
  - user instructions
  - any other project documentation

- `.samples/assets/`

  - templates
  - images
  - design references
  - exported assets
  - any other user-provided resources

## Bootstrap Rules

- Do not start implementation work until the project goal is clear.
- Do not modify project files if the available context is insufficient.
- Do not invent missing requirements.
- Use the provided docs and assets as the source of truth.
- If multiple files conflict, stop and ask the user for clarification.

## If Context Is Missing or Insufficient

Ask the user how they want to proceed:

1. Enter planning mode and generate the missing PRD, specification, or implementation plan.
2. Let the user prepare the missing context in a web client, upload it into `.samples/docs/` or `.samples/assets/`, and continue afterward.

## Completion

Once enough context exists and the initial setup is complete:

1. Remove the first-time setup callout from `AGENTS.md`.
2. Delete this file: `.agents/BOOT.md`.
3. Delete all placeholder data from `README.md` and continue with normal project work.
