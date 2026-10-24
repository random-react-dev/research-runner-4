# Research MCP configuration

Add this connection to your MCP client configuration. Replace `<RESEARCH_TOKEN>` with the token supplied by the owner.

```json
{
  "mcpServers": {
    "research": {
      "type": "http",
      "url": "https://ask-gateway.r95426882.workers.dev/api/research/mcp",
      "headers": {
        "Authorization": "Bearer <RESEARCH_TOKEN>"
      }
    }
  }
}
```
