# No Stairs Please MCP Server

Connect Claude, ChatGPT, and Gemini to the [No Stairs Please MCP server](https://nostairsplease.com/mcp) to search live music venues, booking contacts, room capacities, and show history across all 50 US states, DC, and British Columbia.

Every small stage in all 50 states, and who books it.

## Connection Details

- **Endpoint URL:** `https://nostairsplease.com/mcp`
- **Transport:** Streamable HTTP (stateless)
- **Authentication:** OAuth 2.1 with Dynamic Client Registration
- **Server Card:** `https://nostairsplease.com/.well-known/mcp/server-card.json`
- **Main Directory:** [https://nostairsplease.com/venues](https://nostairsplease.com/venues)
- **Musician Guides:** [https://nostairsplease.com/resources](https://nostairsplease.com/resources)

## Supported Tools

1. **search_venues**: Filter 38,223 open rooms by state, town, category, capacity, music night, or text query.
2. **get_venue**: Read the public details for a single venue by ID.
3. **reveal_venue**: Spend one free reveal to unlock full booking contact details for 7 days.
4. **find_by_performer**: Look up rooms where a band or solo act has played or has upcoming dates.
5. **get_profile**: Check your signed-in account tier, All Access status, and remaining free reveals.
6. **list_saved_venues**: View your saved favorite venues.
7. **save_venue**: Save a venue to your favorites list.
8. **remove_saved_venue**: Remove a venue from your favorites list.

## Example Prompts

- "Find small music venues under 300 capacity in Montana and Idaho with Thursday live music."
- "Which rooms in Austin have booked touring folk or indie acts in the last 90 days?"
- "Save these five Midwest club stops to my No Stairs Please favorites."

## Pricing and Access

You can get started for free with no card needed. Free accounts include monthly venue reveals. One-time All Access passes ($25 for one month or $200 for one year) unlock unlimited venue records across the directory and MCP server.
