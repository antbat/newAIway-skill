# newAIway

newAIway is a business expert for Claude and ChatGPT. It leads a founder or an
owner step by step from an idea to the future state of a working company:
business processes, tasks, staff, AI agents, and an online shop with payments.
It can also evaluate a business idea, or describe an existing business and show
its gaps and weaknesses.

## What is inside

| Part | What it does |
|---|---|
| `skills/newaiway/SKILL.md` | The business-expert skill. It asks one question at a time and saves each answer in newAIway. |
| `.mcp.json` (Claude), `mcp.json` (ChatGPT) | Connects the AI client to the newAIway MCP server at `https://mcp.newaiway.com/`. |

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
`https://mcp.newaiway.com/`. After the plugin is listed in the Claude
directory, you can add it from there too.

**ChatGPT** — add a connector with the URL `https://mcp.newaiway.com/`.

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
