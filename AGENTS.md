# TapKit Docs

Mintlify source for docs.tapkit.ai. Pages are MDX with `title` and `description` frontmatter; navigation lives in `docs.json`.

## Sources of truth

Document what ships, verified against code. When the docs and the code disagree, the code wins.

- Mac app (setup flow, UI copy, what actions the Mac can execute): `../joots-host`
- REST API (`api.tapkit.ai/v1`): `../joots-server/src/jootsing_server/routes/`, `models.py`
- MCP server (`mcp.tapkit.ai/mcp`), tool list and auth: `../tapkit-mcp/src/tools.ts`, `src/mcp-auth.ts`
- Plugins: `../tapkit-plugins-claude`, `../tapkit-plugins-codex`; skills: `../skills` (`master`)
- Web app (tapkit.ai dashboard): `../joots-webapp/src/app/dashboard/`

Read published branches (`origin/main`/`origin/master`), not whatever is checked out locally.

## Rules

- Only document an API endpoint or MCP tool if the Mac app actually executes it (`joots-host/Jootsing/Features/Operation/`). The server has many legacy routes that no longer work.
- Don't document the Python SDK, server-side agent sessions, or Shortcuts-based actions. They are gone.
- Don't quote prices; link to the web app instead.
- Use exact UI labels from the apps, in bold.
- Second person, short sentences, language tags on code blocks, relative links for internal pages.
