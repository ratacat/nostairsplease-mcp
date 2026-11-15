# No Stairs Please MCP Server

Documentation, server card metadata, and client setup examples for the [No Stairs Please MCP server](https://nostairsplease.com/mcp).

Every small stage in all 50 states, and who books it.

## Overview

The No Stairs Please remote MCP server connects Claude, ChatGPT, and Gemini to a live music venue booking directory covering 38,223 open rooms across all 50 US states, the District of Columbia, and British Columbia. Musicians and tour managers use it to look up booking contacts, room capacities, music nights, and 90-day show history.

- **MCP Endpoint:** `https://nostairsplease.com/mcp`
- **Transport:** Stateless Streamable HTTP
- **Authentication:** OAuth 2.1 (`https://nostairsplease.com/.well-known/oauth-protected-resource`)
- **Server Card:** [server-card.json](https://nostairsplease.com/.well-known/mcp/server-card.json)
- **Venue Directory:** [No Stairs Please Venues](https://nostairsplease.com/venues)

## Available Tools

| Tool | Purpose |
|---|---|
| `search_venues` | Search live music venues by state, town, category, capacity, music day, or text query. |
| `get_venue` | Read the venue record for a single room by ID. |
| `reveal_venue` | Spend one free reveal to unlock the full venue record for 7 days. |
| `find_by_performer` | Find venues where a band or solo performer has played or is scheduled to play. |
| `get_profile` | Inspect the signed-in account tier, All Access status, and remaining free reveals. |
| `list_saved_venues` | List the signed-in account's favorite venues. |
| `save_venue` | Add a venue to the signed-in account's favorites list. |
| `remove_saved_venue` | Remove a venue from the signed-in account's favorites list. |

## Client Setup

Add the remote MCP endpoint `https://nostairsplease.com/mcp` in your MCP client and complete the OAuth 2.1 sign-in flow:

```json
{
  "mcpServers": {
    "nostairsplease": {
      "type": "http",
      "url": "https://nostairsplease.com/mcp"
    }
  }
}
```

## License

MIT
