# YouTube MCP Server

Uses `yt-dlp` to download subtitles from YouTube. Try it by asking Claude, "Summarize the YouTube video <<URL>>". Requires `yt-dlp` to be installed locally e.g. via Homebrew.

### How do I get this working?

1. Install `yt-dlp` (Homebrew and WinGet both work great here)
1. Clone this repo and run `npm install`
1. macOS: `code ~/Library/Application\ Support/Claude/claude_desktop_config.json`, Windows: `code $env:AppData\Claude\claude_desktop_config.json`
1. Add this block to the `mcpServers` section or make it if it's not there:

```json
{
  "mcpServers": {
    "mcp-youtube": {
      "command": "node",
      "args": ["/path/to/the/place/you/put/mcp-youtube/lib/index.mjs"]
    }
  }
}
```
