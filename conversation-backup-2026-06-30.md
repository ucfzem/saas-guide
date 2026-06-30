# Conversation Backup — 2026-06-30

## Fix: CSS Grid overflow on saas-guide

### Problem
The `<div class="grid md:grid-cols-2 gap-8 mt-12">` in Étape 1 had the same issue as previous flexbox elements: CSS Grid children have `min-width: auto` by default, so a long line in the `<pre><code>` block (`idea-validator.js`) forced the entire grid column to expand, pushing text content to overflow.

### Fix applied in `<style>`
```css
.grid > * { min-width: 0; }

.code-block {
    max-width: 100%;
    min-width: 0;
    overflow: hidden;
}
.code-block pre {
    max-width: 100%;
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    white-space: pre;
}
```

### Files modified
- `index.html` — added `.grid > *` rule and `.code-block`/`.code-block pre` overflow containment

### Commits
- `fba4521` — fix: grid overflow — add min-width:0 on grid children and scroll containment on code blocks

### Vercel deployments
- Production: https://saas-guide-ten.vercel.app
