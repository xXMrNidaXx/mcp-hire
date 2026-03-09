# mcp-hire 🤝

> Hire developers, designers, and marketers without leaving Claude or Cursor.

Stop switching tabs. Stop writing job posts. Just tell Claude what you need.

## Demo

```
You: I need a React developer to build a dashboard. $5K budget, 2 weeks.

Claude: Found 3 matches on RevolutionAI:
  1. Alex M. — 4.9★ React/Next.js, $95/hr, available now
  2. Sarah K. — 4.8★ Full-stack, $85/hr, available in 3 days
  3. Omar T. — 5.0★ React Native, $110/hr, available now

  Want me to send your project details to any of them?
```

One conversation. No tab switching. Talent delivered to your workspace.

## Setup (2 minutes)

**1. Sign up**

Create a free account at [revolutionai.io](https://www.revolutionai.io) and grab your API key from Settings.

**2. Add to Claude Desktop** (`~/Library/Application Support/Claude/claude_desktop_config.json`)

```json
{
  "mcpServers": {
    "revolutionai": {
      "command": "npx",
      "args": ["-y", "@revolutionai/mcp-server"],
      "env": {
        "REVOLUTION_API_KEY": "your-api-key-here"
      }
    }
  }
}
```

**3. Add to Cursor** (`.cursor/mcp.json` in your project or global config)

```json
{
  "mcpServers": {
    "revolutionai": {
      "command": "npx",
      "args": ["-y", "@revolutionai/mcp-server"],
      "env": {
        "REVOLUTION_API_KEY": "your-api-key-here"
      }
    }
  }
}
```

**4. Restart your client.** That's it.

## Available Tools (21 total)

| Tool | What it does |
|------|-------------|
| `searchTalent` | Find freelancers by skill, rate, availability |
| `getProfile` | View detailed profile + reviews |
| `createProject` | Scope a new project with AI help |
| `sendProposal` | Contact a freelancer |
| `getContracts` | List your active contracts |
| `createMilestone` | Set payment milestones |
| `searchJobs` | Browse posted projects (for freelancers) |
| `applyToJob` | Submit a proposal (for freelancers) |
| + 13 more | Contract management, messaging, reviews... |

## Example Prompts

```
# Finding talent
"Find me a UI/UX designer for a SaaS landing page. Budget $2K, 5 days."
"Who's available for Python data pipeline work this week under $100/hr?"
"Show me the top-rated React developers on RevolutionAI."

# Project scoping
"Help me scope a project for building a RAG chatbot with my docs."
"What should I budget for a mobile app MVP in 6 weeks?"

# Managing work
"What's the status of my active contracts?"
"Create a $2K milestone for the first prototype delivery."
"Send a message to my current developer about the API spec."
```

## Why RevolutionAI?

- **Pre-vetted talent** — every freelancer screened for real production experience
- **All skill types** — developers, designers, marketers, copywriters
- **Fast matching** — typically matched within 24 hours
- **MCP-native** — built specifically for AI workspace integration
- **Transparent pricing** — no hidden fees, milestone-based payments

## Talent Categories

- Frontend / Full-stack developers
- Mobile (iOS, Android, React Native)
- AI/ML engineers
- UI/UX designers
- Brand designers
- Growth marketers
- Content writers
- DevOps / Infrastructure

## Pricing

- **Free to browse and post** — no account fee
- **10% platform fee** on client side
- **YC Alumni offer** — first 3 months free for YC companies

## Links

- [Sign up → revolutionai.io](https://www.revolutionai.io)
- [Post a project in 5 min](https://www.revolutionai.io/plan-project)
- [Post a job](https://www.revolutionai.io/plan-job)
- [MCP server docs](https://www.revolutionai.io/docs/mcp)
- [npm: @revolutionai/mcp-server](https://www.npmjs.com/package/@revolutionai/mcp-server)

## Contributing

Found a bug in the MCP server? Want to add a tool? Open an issue or PR.

---

⭐ Star this if it saved you a browser tab. Built by [RevolutionAI](https://www.revolutionai.io).
