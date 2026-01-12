# Copilot Instructions for this Repository ✅

## Project snapshot
- Single static HTML page: `Bài 1.html` (UTF-8 encoded, contains inline CSS). The page is a simple course-card layout using flexbox and pseudo-elements.

## What an AI assistant should know (quick, actionable)
- File of interest: `Bài 1.html` — do not rename the file or remove diacritics without confirming with the maintainer; filenames use Unicode characters.
- There is no build, test, or package system in this repo. Preview changes by opening the HTML in a browser or using VS Code Live Server.
- Encoding: the file uses `charset=utf-8`. Preserve this encoding when editing.

## Common patterns & examples from the codebase
- Inline styles inside a `<style>` tag are used for layout and visual rules. Example pattern:

```css
.course-card { display:flex; flex-direction:column; padding:30px; }
.icon::after { content:'✔'; color:white; font-size:12px; }
```

## Known issues to address (discovered in the current commit)
- The CSS ends with an unfinished rule: `.benefit-item` (missing body and closing braces). Fixes typically are:
  - Close the CSS rule with `}` and ensure the `<style>` block is properly closed.
  - Make sure the HTML structure (e.g., `<body>`, closing tags) is valid and complete.

## How to propose changes (PR guidance)
- Keep changes minimal and focused: one fix per PR (e.g., "Fix CSS syntax and close HTML tags").
- Include a short description of the issue and the verification steps (e.g., browser screenshot or mention of Live Server preview).
- When editing, preserve original diacritics and encoding; explain if you must change filenames.

## Automated checks & validation (recommended actions for changes)
- Manual preview in a browser (or use Live Server) to confirm layout and responsive behavior.
- Quick HTML/CSS linting: run an online validator or a VS Code extension (e.g., "HTMLHint" or "stylelint"). Document any linting rules you follow in the PR.

## When to ask maintainers for clarification
- If you want to rename or move `Bài 1.html` (because it contains non-ASCII characters).
- If you plan to introduce a build or test system—ask first to discuss preferred tools.

---

If you'd like, I can also open a PR that fixes the CSS syntax error and completes the minimal page structure (small, self-contained change). Want me to proceed? 🔧