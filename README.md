# North Metric for Claude Code

[North Metric](https://northmetric.io) predicts which paying customers will churn, drafts a move for each one in the Queue, and proves what each move kept in the Ledger. This plugin connects Claude Code to North Metric's MCP server, so you can ask about churn and act on it from your terminal.

## Install

```bash
claude plugin marketplace add north-metric/claude-plugin
claude plugin install north-metric@north-metric
```

Then start Claude Code, run `/mcp`, choose **north-metric** and sign in to North Metric. On the consent page you pick:

- **Workspace:** the one Claude Code works in.
- **Access:** **Read only**, or **Read and act**, which also drafts, edits, approves, skips and snoozes moves and pauses the Queue. Read and act needs the Approver role or above. Claude Code asks you before each action.
- **Hide customer names and emails:** customers then show by ID only.

You can change these or disconnect any time in North Metric under **Your profile › AI tools**.

## What you can ask

- Who is most likely to churn this month, and why?
- What's waiting in the Queue, and what does each move say?
- How much MRR did approved moves keep, and how does that compare with customers we held back?
- Which customers are on old prices or discounts that never end?

## Other MCP clients

The plugin only adds this server URL to Claude Code. Any MCP client that supports remote servers with sign-in can use it directly:

```
https://app.northmetric.io/mcp
```

Setup for Claude, ChatGPT, Cursor and VS Code: [northmetric.io/integrations/mcp](https://northmetric.io/integrations/mcp).

## Privacy and support

- Privacy: [northmetric.io/privacy](https://northmetric.io/privacy)
- Terms: [northmetric.io/terms](https://northmetric.io/terms)
- Support: [hello@northmetric.io](mailto:hello@northmetric.io)
