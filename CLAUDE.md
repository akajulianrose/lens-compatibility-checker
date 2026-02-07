# Lens Compatibility Checker

## Project Overview
A static web app for cinematographers to check lens mount-to-camera mount compatibility. Users select a lens mount and camera mount from dropdowns and get immediate visual feedback (compatible, incompatible, edge case, or same mount) with detailed notes and links to adapters on Amazon.

## Tech Stack
- Single-file static HTML/CSS/JS (no framework, no build step)
- Hosted on Vercel (planned)
- No backend or database — all compatibility data lives in a JS object in `index.html`

## File Structure
- `index.html` — the entire app (markup, styles, and logic)
- `CLAUDE.md` — this file

## Design Principles
- Apple "liquid glass" aesthetic (frosted glassmorphism, subtle transparency, soft glows)
- Light and dark mode support (toggle + system preference detection)
- Light mode: white-to-gray gradient background
- Dark mode: charcoal-to-black gradient background
- Status indicator uses translucent colored glass circles, not opaque flat colors
- Keep the UI minimal and focused — no clutter

## Supported Mounts
Canon EF, Canon RF, Sony E, Nikon F, Nikon Z, Micro Four Thirds, L-Mount, Fuji X, PL (Cinema)

## Monetization
- Amazon search links on compatible combinations (placeholder for future affiliate IDs)
- Amazon button uses a blue gradient style

## Git Conventions
- Write clear, concise commit messages that explain *why*, not just *what*
- Use conventional-style prefixes: `feat:`, `fix:`, `style:`, `refactor:`, `docs:`, `chore:`
- Keep commits atomic — one logical change per commit
- Never force push to `main`
- Never commit secrets, API keys, or credentials
- Always review staged changes before committing
- Do not amend previous commits unless explicitly asked
- Do not skip pre-commit hooks unless explicitly asked

## Future Plans
- Deploy to Vercel
- Add Amazon affiliate IDs to adapter links
- Expand mount database (more mounts and combinations)
- Potentially add flange distance reference info
- Consider migrating to a framework if complexity grows
