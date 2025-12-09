# AGENTS.md

## Project overview
- This repository is a very simple static site.
- The primary file is `index.html` in the repository root.
- The repo is used mainly as a test host for GitHub Pages / static HTML.

## How to work in this repo
- Only edit `index.html` unless the user explicitly asks for additional files.
- Always read the current `index.html` from the repository before making changes.
- Apply changes **surgically**:
  - Preserve existing structure, IDs, classes, comments, and content unless the user requests changes.
  - Avoid rewriting the entire file when only a small change is requested.
- Keep indentation consistent (2 spaces) and use Unix line endings (`\n`).
- Use plain, semantic HTML. Do not introduce build tools, frameworks, or bundlers unless explicitly requested.

## Testing instructions
- This project does **not** have an automated test suite.
- Do **not** run `npm test`, `yarn test`, `pytest`, or other test commands.
- Instead, “testing” for this repo means:
  - Ensuring the HTML is well-formed (no unclosed or mis-nested tags).
  - Making sure links, IDs, and anchors are valid and consistent.
- When summarizing your work, explicitly note:  
  - **Automated tests:** not applicable (static HTML project with no test suite).

## Git / PR behavior
- Use the `main` branch as the base branch unless the user specifies otherwise.
- For each task, create a new branch with a descriptive name, e.g.:
  - `codex/index-html-update-<short-description>`
- Before committing:
  - Re-read `index.html` from disk to incorporate any upstream changes.
  - Resolve differences by **merging** with the existing content rather than replacing the whole file.
- Keep commits small and focused on the requested changes.
- In the PR description, include:
  - A brief summary of the visible changes to `index.html`.
  - A note that there is no automated test suite and that changes were validated by manual HTML review.

## Style and content guidelines
- Keep the page simple; this repository is primarily a test/demo host.
- Avoid adding heavy dependencies (no React/Vue/build steps) unless explicitly asked.
- Prefer:
  - Plain HTML
  - Minimal inline CSS or a single small `<style>` block
  - No unnecessary JavaScript
