# Inspora plugin

Design-inspiration search from the Inspora catalog inside Claude Code and Codex. The plugin adds the hosted Inspora MCP (`https://mcp.inspora.design/mcp`) and two skills, `inspora-discovery` and `inspora-design-direction`.

The plugin holds no credentials. Access requires signing in with an approved Inspora account; it is currently limited to the Inspora team.

## Claude Code

Inside Claude Code:

```
/plugin marketplace add inspora-design/inspora-plugin
/plugin install inspora@inspora-team
```

Then run `/reload-plugins` and `/mcp`, select `plugin:inspora:inspora`, choose **Authenticate** and sign in to Inspora.

## Codex

```bash
codex plugin marketplace add inspora-design/inspora-plugin
codex plugin add inspora@inspora-team
```

If `codex mcp list` shows **Not logged in** for `inspora`, run `codex mcp login inspora`.

Full setup, including removing an earlier manual setup and other agents: [mcp.inspora.design/setup](https://mcp.inspora.design/setup).

This repository is published from the Inspora source repository; changes made here directly are overwritten on the next release.
