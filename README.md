# Expo monorepo template

Next.js web + Expo mobile in a pnpm workspace, with Claude Code config, ready for a new idea.

- **Skills**: Vercel (`vercel-labs/agent-skills`) and Matt Pocock (`mattpocock/skills`) in `.claude/skills`, pinned in `skills-lock.json`.
- **Plugins**: impeccable, ponytail and expo, via `.claude/settings.json` (auto-updating marketplaces).
- **MCP**: lazyweb, via `.mcp.json`. Export `LAZYWEB_API_KEY` in your shell.
- **Updates**: Dependabot runs daily and green PRs auto-merge (Expo SDK packages excluded); `Update skills and Expo` workflow refreshes skills and runs `expo install expo@latest --fix` daily. Both land on `main`.

## Start

1. **Use this template** on GitHub, clone, `pnpm install`.
2. Import the repo in Vercel with root directory `apps/web` so `main` deploys to production.
3. Open Claude Code; the first-run block in `AGENTS.md` takes it from there.

`apps/mobile` is Expo for now; native `apps/ios` and `apps/android` can replace it later, so keep shared logic outside it.
