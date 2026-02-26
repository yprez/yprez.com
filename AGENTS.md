# yprez.com

Personal portfolio site for Yuri Prezument. Single-page static site deployed via GitHub Pages at yprez.com.

> **Note:** `CLAUDE.md` is a symlink to this file (`AGENTS.md`). Edit `AGENTS.md` directly.

## General guidelines

- When suggesting changes to a file, prefer breaking them into smaller chunks
- Never tell the user "you're absolutely right" or similar affirmations
- Maintain single-file architecture -- all HTML, CSS, and JS live in `index.html`
- Act autonomously on reversible changes; ask before changing the domain or deployment setup
- Do not open files with xdg-open -- the user will preview in their own browser

## Constraints

- Vanilla HTML, CSS, and JavaScript only -- no frameworks, no build tools, no package manager
- No external dependencies -- no CDN fonts, no external CSS/JS beyond the analytics script
- No cookies -- use localStorage only if needed
- CSS custom properties for theming (light/dark) -- keep the existing variable naming
- JavaScript uses the IIFE pattern for encapsulation
- Accessibility: skip-to-content link, semantic HTML, ARIA attributes where needed
- Analytics: external script from analytics.codequalitycheck.com (do not remove or change the website ID)

## Development

```bash
# Open directly in browser
xdg-open index.html

# Or use a local server
python -m http.server 8000
```

No build step. No tests. Manual browser testing only.

## Deployment

GitHub Pages from the `main` branch. The `CNAME` file maps to `yprez.com`. Push to main to deploy.

## Git standards

- Commit messages should be concise and descriptive
- Never add AI attribution or co-authorship markers to commits
