# newAIway

newAIway is a Human/AI collaboration platform: one home for small, focused AI
products (LifeTimePriceless, ClearDomain, Assistant8, time08, OrgKnowledge,
aiOrgBoard), with one account and one subscription. This plugin teaches Claude
and ChatGPT what newAIway and each product are.

## What is inside

| Part | What it does |
|---|---|
| `skills/newaiway/SKILL.md` | Explains newAIway and gives one paragraph about each product. |
| `.mcp.json` (Claude), `mcp.json` (ChatGPT) | Connects the AI client to the newAIway MCP server at `https://api.newaiway.com/mcp`. |

## What it connects to, and what it sends

- The plugin runs no code on your machine. It only adds the skill and the
  remote MCP server.
- The MCP server is the newAIway service. You sign in to newAIway with OAuth,
  choose one company, and approve the access.
- The AI client then reads and changes that company's records — for example
  the company name, wiki pages, tasks, positions and products — with the
  permissions of your role in that company. Tools named `delete_` cannot be
  undone.
- The plugin sends data to no other place.

You need a newAIway account. Create one at <https://my.newaiway.com>.

## Install

**Claude Code**

```bash
claude plugin marketplace add antbat/newAIway-skill
claude plugin install newaiway@newaiway
```

**Claude (claude.ai, Desktop)** — add a custom connector with the URL
`https://api.newaiway.com/mcp`. After the plugin is listed in the Claude
directory, you can add it from there too.

**ChatGPT** — add a connector with the URL `https://api.newaiway.com/mcp`.

To disconnect an AI client, open newAIway → Settings → Connected assistants.

## Links

- Privacy Policy: <https://newaiway.com/privacy/>
- Terms of Service: <https://newaiway.com/terms/>
- Support: <https://newaiway.com/support/> · info@newaiway.com

## License

PolyForm Noncommercial 1.0.0, with one additional permission: you may use this
plugin for any purpose, commercial purposes included, when you use it with the
newAIway service. You may not reuse its contents in another product for a
commercial purpose. See [LICENSE](LICENSE).
