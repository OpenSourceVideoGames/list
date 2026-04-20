# AGENTS.md

This repository is a curated Markdown list, not an application. Most work here is editorial, but it still needs strict validation because small mistakes create bad pull requests and noisy diffs.

## Repository Purpose

- Maintain `README.md` as a categorized list of open source video games and game-related projects.
- Keep entries in the correct section and sorted consistently with the rest of the list.
- Prefer small, single-purpose pull requests.

## Source of Truth

- The only file that normally changes is `README.md`.
- Use the current upstream `master` branch as the base for new work.
- Before editing, inspect the surrounding section to match local formatting exactly.

## Entry Requirements

Only add a repository when all of the following are true:

- It is actually a game, game-related project, or game engine/framework suitable for this list.
- The source code is publicly available.
- The repository is relevant to the target section.
- The title in `README.md` should match the repository or project name as presented by the project, with obvious cosmetic cleanup when needed.

Do not add entries that are:

- Duplicates of existing items.
- Clearly unrelated to games.
- Closed-source games with only marketing pages.
- Entries placed in the wrong category just because they use a certain language or engine.

## Play It Now Policy

- Add a `Play it now!` link only when there is a real public playable page.
- A playable link should let a user launch or access the game directly, not just view the repository, store page, or documentation.
- If no suitable public playable link exists, omit `Play it now!`.
- Re-check playable links carefully for VR entries, because many repositories are source-only student or prototype projects.

## Language and Engine Notes

When adding implementation details:

- Prefer `Written in ...` only when that phrasing already fits the section style or the requested contribution style.
- If the project is built with a recognizable game engine, name the engine instead of only naming the host language.
- Example: prefer `Written in Unity` over `Written in C#` for a Unity project.

## Sorting and Formatting

- Keep entries alphabetically sorted by visible project name within their section.
- Follow existing Markdown bullet style exactly: `* [Name](url) - Description.`
- Preserve existing punctuation and sentence casing patterns around neighboring entries.
- Remove unnecessary hyphens from names when the repository README or project branding clearly uses a spaced or plain form instead.

## Validation Checklist

Before opening or updating a PR:

1. Confirm the repository is genuinely open source and game-related.
2. Confirm it is not already present elsewhere in `README.md`.
3. Confirm the section is correct.
4. Confirm alphabetical ordering.
5. Confirm any `Play it now!` link is real and public.
6. Diff against upstream and ensure the PR contains only the intended entry change.

## PR Hygiene

- Avoid batching unrelated additions into one pull request.
- Rebase or rebuild stale branches on top of current upstream `master` before pushing.
- Watch for accidental carry-over entries from previous work.
- If a PR diff contains anything beyond the intended addition or correction, rebuild it from a clean upstream base.

## Working Style

- Prefer deterministic checks over assumptions.
- When reviewing issue-driven additions, verify each repository manually instead of trusting issue text.
- If there is ambiguity about whether something is a game, a framework, or not suitable for the list, document the reasoning in the PR description or keep it out until verified.
