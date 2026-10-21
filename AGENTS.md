# Project agent memory

This file is the project's committed home for project-intrinsic agent knowledge: build, test, release, architecture, and sharp-edge notes that should travel with the code.

- The whole site is `index.html`: static HTML, inline CSS and vanilla JS, no build step and no JS libraries. It is served by Cloudflare Pages at https://mi-tech.pages.dev/; that URL is repeated in the canonical, Open Graph and JSON-LD tags in the `<head>`.
- Folder layout and how to add a project card: see `README.md`. Screens are WebP pairs (`<screen>.webp` for the viewer, `<screen>-600.webp` for the card); every `<img>` carries width/height and below-the-fold images lazy-load.
- Copy rules from the owner: call the voice co-rider project "Kora" and nothing else; never use an earlier working name for it anywhere (text, alt text, commits, PRs). Every claim on a card (role, hackathon, release, stack) must be backed by that project's repo; no invented metrics.
- Content stays visible without JS: scroll reveals, the intro screen and the custom cursor are added by script and skipped under `prefers-reduced-motion`. Keep it that way when adding motion.
- Check changes in a browser at phone (390px) and desktop (1440px) widths, in light and dark themes, before opening a PR.

## Maintaining this file

Keep this file for knowledge useful to almost every future agent session in this project.
Do not repeat what the codebase already shows; point to the authoritative file or command instead.
Prefer rewriting or pruning existing entries over appending new ones.
When updating this file, preserve this bar for all agents and keep entries concise.
