# Space Base Race — Claude Code Guidelines

## Permissions Model

### Full autonomy (no confirmation needed)
- Edit any file in this repo (`index.html`, `readme.md`, assets, configs)
- Run the dev server (`npx serve`)
- `git add`, `git commit`, `git push` to the `dev` branch
- Create GitHub PRs from `dev` → `main`
- Read files, run grep/find, take screenshots via preview tools
- Install dev tooling locally (linters, formatters) if needed

### Always ask for confirmation
- `git push` to `main` directly (bypassing PR)
- Merging any PR into `main` — user must approve the merge
- Deleting branches or force-pushing anything
- Any action that modifies the live itch.io deployment

## Branch Strategy
- `dev` — active development, Claude works freely here
- `main` — production, deployed to itch.io; merges require explicit user approval

## Project Context
- Single-file React 18 app (`index.html`) — no build step
- All game logic, UI, and audio live in `index.html`
- `readme.md` changelog and in-game `PATCH_NOTES` array must stay in sync
- Preview server runs via `npx serve` on port 8080
- GitHub repo: `spacebaserace/spacebaserace`
