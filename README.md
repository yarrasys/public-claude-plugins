# Yarra Systems — Claude Code plugins

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) published by
**Yarra Systems**.

## Use it

```
/plugin marketplace add yarrasys/public-claude-plugins
/plugin install yarradev-board@yarrasys
```

(`@yarrasys` is the **marketplace** name declared in `.claude-plugin/marketplace.json`, not the plugin
name.)

## Plugins

| Plugin | What it does |
|---|---|
| [**yarradev-board**](./yarradev-board) | An agent-native SDLC orchestrator — a reconciliation-loop skill + role subagents (designer → developer → tester, plus a security-advisor, a releaser staging deploy, and a human production gate) that drive a yarradev HTTP board through a gated lifecycle (`spec→dev→test→done→staging→prod`), running on **your own Claude subscription**. See its [README](./yarradev-board/README.md). |

> ⚠️ `yarradev-board` is the open **client**. Its HTTP board backend (the `yarradev-platform` Cloudflare
> service) is a separate, not-yet-public service — without a board endpoint to point it at, only the
> plugin's offline `npm test` suite runs standalone.

## License

MIT © 2026 Yarra Systems — see [LICENSE](./LICENSE). Each plugin also carries its own license file.
