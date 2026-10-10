# Ads Libraries MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/ads-libraries)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Connect Ads Libraries to AI assistants: competitor ad research across Meta, Google, LinkedIn, Microsoft and TikTok ad libraries.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — use Ads Libraries from Claude, ChatGPT, Cursor, and other AI assistants through the Model Context Protocol (MCP).

<img src="images/ads-libraries-icon.svg" alt="Ads Libraries MCP Server" width="64" height="64">

## MCP Server URL

```
https://ads-libraries.insightfulmcp.com/
```

## What is Ads Libraries MCP?

Ads Libraries MCP is a **remote Model Context Protocol server** hosted by InsightfulPipe. Access ad transparency data and creative libraries across platforms to research competitor campaigns and market trends.

## Installation

### Claude

1. Copy the MCP Server URL: `https://ads-libraries.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** and sign in to InsightfulPipe if asked. Claude then lists the connector as connected.

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://ads-libraries.insightfulmcp.com/`
3. Sign in to InsightfulPipe if asked. The connection finishes as soon as you are signed in.

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http ads-libraries https://ads-libraries.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "ads-libraries": {
      "url": "https://ads-libraries.insightfulmcp.com/"
    }
  }
}
```

When Cursor shows **Needs authentication**, click **Connect** and sign in to InsightfulPipe if asked.

## Available Actions

17 actions: 17 read, 0 write.

### Read Actions (17)

| Action | Description |
|--------|-------------|
| `facebook_company_ads` | Get all ads from a specific Facebook page/company |
| `facebook_search_ads` | Search Facebook Ads Library by keyword |
| `facebook_search_companies` | Search for Facebook companies/pages to get their page_id |
| `google_ad_details` | Get detailed information about a specific Google ad |
| `google_company_ads` | Get all ads for a company from Google Ads Transparency |
| `google_search_advertisers` | Search for advertisers in Google Ads Transparency Center |
| `linkedin_ad_details` | Get detailed information about a specific LinkedIn ad |
| `linkedin_search_ads` | Search LinkedIn Ad Library |
| `microsoft_advertiser_ads` | Get all ads from a specific Microsoft advertiser |
| `microsoft_get_ad` | Get a specific Microsoft ad by ID |
| `microsoft_get_advertiser` | Get a specific Microsoft advertiser by ID |
| `microsoft_list_countries` | List available country codes for Microsoft Ads filtering |
| `microsoft_search_ads` | Search Microsoft Ads Library |
| `microsoft_search_advertisers` | Search for Microsoft advertisers by name |
| `tiktok_ad_details` | Get targeting, reach and creative details for a TikTok Ad Library ad |
| `tiktok_search_ads` | Search TikTok Ad Library (ads shown in the EU, EEA, UK, Switzerland and Turkey) |
| `tiktok_top_ads` | Get TikTok's top-performing ads from Creative Center |

## Control What Your AI Can Do

You decide what AI agents can do with each connected account:

- **Turn individual actions on or off** for every connected account, so agents only see the actions you allow.
- **Connect as Read-only or Read & Write.** A read-only connection can only enable read actions.
- **Destructive actions stay off by default.** Actions such as deletes are disabled until an admin enables them.
- **Team access per account.** Restricted team members only use the accounts they are granted, with the read actions enabled on them.

## Usage Examples

```
"Show active Facebook ads from a competitor's page"
```

```
"Find LinkedIn ads that mention "marketing analytics""
```

```
"Look up the Google ads a competitor domain is running"
```

```
"Show the top TikTok ads in beauty in the US over the last 30 days"
```

## Pricing

The Ads Libraries MCP server is included in every InsightfulPipe plan, together with all other MCP servers and the CLI. Plans start at $29.99/month, and you can try it for 7 days. See [insightfulpipe.com/pricing](https://insightfulpipe.com/pricing) for current plans.

## Ready-Made Skills and Prompts

- [Competitor Facebook Ad Research](https://insightfulpipe.com/marketing-prompts-library/ads-libraries-competitor-facebook-ad-research)
- [Google Ads Transparency Research](https://insightfulpipe.com/marketing-prompts-library/ads-libraries-google-ads-transparency-research)
- [Multi Platform Ad Audit](https://insightfulpipe.com/marketing-prompts-library/ads-libraries-multi-platform-ad-audit)

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers.

- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads)
- [Meta Ads MCP](https://insightfulpipe.com/mcp-servers/facebook-ads)
- [LinkedIn Ads MCP](https://insightfulpipe.com/mcp-servers/linkedin-ads)
- [TikTok Ads MCP](https://insightfulpipe.com/mcp-servers/tiktok-ads)

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-ads-libraries)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blog)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.
