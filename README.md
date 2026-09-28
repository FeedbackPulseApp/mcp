# FeedbackPulse MCP

Remote Model Context Protocol server for [FeedbackPulse](https://feedbackpulse.com/).

**Endpoint:** `https://app.feedbackpulse.com/mcp`  
**Docs:** https://feedbackpulse.com/help/integrations/mcp-overview/

## Install (Claude Code)

```bash
claude mcp add feedbackpulse \
  --transport http \
  https://app.feedbackpulse.com/mcp \
  --header "Authorization: Bearer YOUR_TOKEN"
```

Create a personal API token in FeedbackPulse as Admin under **Settings → Integrations**.

## Install (Claude Desktop / Claude.ai)

Use OAuth. Follow:

- https://feedbackpulse.com/help/integrations/connect-claude-desktop/
- https://feedbackpulse.com/help/integrations/connect-claude-ai/

## Manual client config (HTTP + Bearer)

```json
{
  "mcpServers": {
    "feedbackpulse": {
      "url": "https://app.feedbackpulse.com/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_TOKEN"
      }
    }
  }
}
```

## Official MCP Registry

Remote entry is defined in [`server.json`](./server.json) as `com.feedbackpulse/mcp`.

## Related

Cursor Marketplace survey-design plugin (separate MCP path): https://github.com/FeedbackPulseApp/cursor-employee-surveys-plugin

## License

MIT
