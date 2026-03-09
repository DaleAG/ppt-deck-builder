# HTML Prototyping and Export

## When to use HTML/CSS
Prefer HTML/CSS when:
- the deck has lots of Chinese text
- the user wants stable iteration
- layout and wording will change frequently
- the user wants editable output instead of generated images

## Build rules
- Keep a single HTML file for fast global edits when possible.
- Use CSS variables for theme color.
- Keep fixed slide dimensions.
- Reuse layout blocks through semantic class names.

## Iteration rules
- First fix structure.
- Then fix visual hierarchy.
- Then do brand/theme upgrades.

## PDF export pitfalls
### Symptom
Right side gets cut off or page scaling breaks.

### Cause
Browser print uses default paper instead of the slide canvas.

### Fix
Use print rules such as:
- `@page { size: 1366px 768px; margin: 0; }`
- `@media print` to remove extra spacing, shadows, and borders
- force each slide to page-break cleanly

## Local preview
Use a local HTTP server instead of `file://` when browser tooling blocks local files.

Example:
- `python -m http.server 8765`
- open `http://127.0.0.1:8765/<file>.html`
