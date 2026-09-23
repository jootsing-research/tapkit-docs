# TapKit Docs

Source for [docs.tapkit.ai](https://docs.tapkit.ai).

## Local development

```
npm i -g mint
mint dev
```

Preview at `http://localhost:3000`. Check links with `mint broken-links`.

## Structure

| Tab | Path | What's there |
|-----|------|--------------|
| Documentation | root | Introduction, setup, Mac app, web app, security |
| Integrations | `integrations/` | Claude, Codex, MCP, skills |
| API Reference | `api-reference/` | REST endpoints |

## Deploying

Pushes to `main` deploy automatically via Mintlify.
