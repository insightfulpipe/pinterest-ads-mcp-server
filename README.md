# Pinterest Ads MCP Server by Insightful Pipe

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/pinterest-ads)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Connect Pinterest Ads to AI assistants for visual advertising analytics and shopping campaign optimization.**

Part of the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — The Pinterest Ads MCP server enables Claude, ChatGPT, Cursor, and other AI assistants to analyze your Pinterest advertising campaigns. Optimize visual marketing, track shopping performance, and get AI-powered recommendations.

[![Explore All MCP Servers](https://img.shields.io/badge/Explore_All-MCP_Servers-blue?style=for-the-badge)](https://insightfulpipe.com/mcp-servers)

![Pinterest Ads MCP Server](https://insightfulpipe.com/images/pinterest-round-color-icon.svg)

## MCP Server URL

```
https://pinterest-ads.insightfulmcp.com/
```

## What is Pinterest Ads MCP?

Pinterest Ads MCP is a **remote Model Context Protocol server** that connects your Pinterest Business account to AI assistants. This visual marketing integration allows you to:

- Query Pinterest ad performance using natural language
- Analyze pin engagement and shopping metrics
- Track ROAS for catalog and shopping campaigns
- Access audiences, catalogs, and audience insights
- Generate async analytics reports

## Installation

### Claude

1. Copy the MCP Server URL: `https://pinterest-ads.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://pinterest-ads.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http pinterest-ads https://pinterest-ads.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "pinterest-ads": {
      "url": "https://pinterest-ads.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Actions

44 actions: 28 read, 16 write.

### Read Actions (28)

<details>
<summary>Show all 28 read actions</summary>

| Action | Description |
|--------|-------------|
| `get_ad` | Get details for a specific ad |
| `get_ad_account` | Get details for a specific ad account |
| `get_ad_account_analytics` | Get analytics for an ad account |
| `get_ad_accounts` | List all ad accounts accessible to the user |
| `get_ad_analytics` | Get analytics for ads |
| `get_ad_group` | Get details for a specific ad group |
| `get_ad_group_analytics` | Get analytics for ad groups |
| `get_ad_groups` | List ad groups for an ad account |
| `get_ads` | List ads for an ad account |
| `get_audience` | Get details for a specific audience |
| `get_audience_insights` | Get audience insights for an ad account |
| `get_audiences` | List audiences for an ad account |
| `get_campaign` | Get details for a specific campaign |
| `get_campaign_analytics` | Get analytics for campaigns |
| `get_campaigns` | List campaigns for an ad account |
| `get_catalog_feeds` | List catalog feeds |
| `get_catalogs` | List catalogs for the authenticated user |
| `get_conversion_tag` | Get details for a specific conversion tag |
| `get_conversion_tags` | List conversion tags for an ad account |
| `get_customer_list` | Get details for a specific customer list |
| `get_customer_lists` | List customer lists for an ad account |
| `get_keywords` | List keywords for an ad account |
| `get_pin` | Get details for a specific pin |
| `get_report` | Get the status or download an async report |
| `get_targeting_analytics` | Get targeting analytics breakdown for an ad account |
| `get_trending_keywords` | Get trending keywords for a region |
| `get_user_account` | Get the authenticated user's account information |
| `get_user_account_analytics` | Get analytics for the authenticated user's account |

</details>

### Write Actions (16)

| Action | Description |
|--------|-------------|
| `create_ad_groups` | Create ad groups for an ad account (always created in PAUSED status for safety) |
| `create_ads` | Create ads for an ad account (always created in PAUSED status for safety) |
| `create_audience` | Create an audience for an ad account |
| `create_campaigns` | Create campaigns for an ad account (always created in PAUSED status for safety) |
| `create_conversion_tag` | Create a conversion tag for an ad account |
| `create_customer_list` | Create a customer list for an ad account |
| `create_customer_list_upload` | Create a customer list upload for an existing customer list |
| `create_keywords` | Create keywords for an ad account |
| `create_report` | Create an async analytics report |
| `run_customer_list_upload` | Run a previously created customer list upload |
| `update_ad_groups` | Update ad groups for an ad account |
| `update_ads` | Update ads for an ad account |
| `update_audience` | Update an audience for an ad account |
| `update_campaigns` | Update campaigns for an ad account |
| `update_customer_list` | Update a customer list for an ad account |
| `update_keywords` | Update keywords for an ad account |

## Usage Examples

### Campaign Performance

```
"How are my Pinterest ad campaigns performing this month?"
```

### Shopping Analytics

```
"Which products are getting the most saves from Pinterest?"
```

### Ad Performance

```
"Show me my top performing Pinterest ads by engagement"
```

### Trending Keywords

```
"What keywords are trending in the home decor category?"
```

### Audience Insights

```
"Get audience insights for my ad account"
```

## Supported Metrics

| Metric | Description |
|--------|-------------|
| Impressions | Total pin views |
| Pin Clicks | Clicks on pins |
| Outbound Clicks | Clicks to your website |
| Saves | Pins saved to boards |
| Closeup Views | Pin detail views |
| Add to Cart | Shopping cart adds |
| Checkout | Completed purchases |
| ROAS | Return on ad spend |

## Why Pinterest Ads MCP?

### For E-commerce Brands
- **Shopping insights** - Product-level performance
- **Catalog analytics** - Product feed performance
- **Trending discovery** - Find trending keywords

### For Lifestyle Brands
- **Inspiration tracking** - See how content inspires
- **Seasonal trends** - Capitalize on Pinterest trends

### For Agencies
- **Multi-account management** - Handle client accounts
- **Async reporting** - Generate detailed reports
- **Cross-platform comparison** - Pinterest vs other channels

## Security & Privacy

- **Official Pinterest API** - Direct integration with Pinterest's API
- **OAuth 2.0** - Secure authentication
- **Granular permissions** - Control access level
- **Data encryption** - Secure transmission

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers for marketing and analytics.

### Visual & E-commerce MCP Servers
- [Instagram MCP](https://insightfulpipe.com/mcp-servers/instagram) - Visual social analytics
- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads) - Search + Shopping ads
- [Facebook Ads MCP](https://insightfulpipe.com/mcp-servers/facebook-ads) - Social advertising

### Social Advertising MCP Servers
- [TikTok Ads MCP](https://insightfulpipe.com/mcp-servers/tiktok-ads) - Video advertising
- [Snapchat Ads MCP](https://insightfulpipe.com/mcp-servers/snapchat-ads) - Gen-Z advertising

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs/connectors-pinterest-ads)
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
