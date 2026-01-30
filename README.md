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
- Access boards, pins, and audience insights
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

1. Copy the MCP Server URL: `https://pinterest-ads.insightfulmcp.com/`
2. Open ChatGPT Settings → **Connections**
3. Click **Add Connection** and paste the URL
4. Authorize with your InsightfulPipe account

### Claude Code

```bash
claude mcp add pinterest-ads https://pinterest-ads.insightfulmcp.com/
```

### Cursor

1. Open Cursor Settings → **MCP Servers**
2. Add new server with URL: `https://pinterest-ads.insightfulmcp.com/`
3. Authorize the connection

## Available Actions

| Action | Description |
|--------|-------------|
| `get_ad_account` | Get details for a specific ad account |
| `get_ad_accounts` | List all ad accounts accessible to the user |
| `get_campaigns` | List campaigns for an ad account |
| `get_campaign` | Get details for a specific campaign |
| `get_ad_groups` | List ad groups for an ad account |
| `get_ad_group` | Get details for a specific ad group |
| `get_ads` | List ads for an ad account |
| `get_ad` | Get details for a specific ad |
| `get_audiences` | List audiences for an ad account |
| `get_audience` | Get details for a specific audience |
| `get_conversion_tags` | List conversion tags for an ad account |
| `get_conversion_tag` | Get details for a specific conversion tag |
| `get_customer_lists` | List customer lists for an ad account |
| `get_customer_list` | Get details for a specific customer list |
| `get_keywords` | List keywords for an ad account |
| `get_boards` | List boards for the authenticated user |
| `get_board` | Get details for a specific board |
| `get_board_sections` | List sections for a board |
| `get_board_pins` | List pins on a board |
| `get_board_section_pins` | List pins in a board section |
| `get_pin` | Get details for a specific pin |
| `get_catalogs` | List catalogs for the authenticated user |
| `get_catalog_feeds` | List catalog feeds |
| `get_user_account` | Get the authenticated user account information |
| `get_ad_account_analytics` | Get analytics for an ad account |
| `get_campaign_analytics` | Get analytics for campaigns |
| `get_ad_group_analytics` | Get analytics for ad groups |
| `get_ad_analytics` | Get analytics for ads |
| `get_targeting_analytics` | Get targeting analytics breakdown for an ad account |
| `get_user_account_analytics` | Get analytics for the authenticated user account |
| `get_audience_insights` | Get audience insights for an ad account |
| `get_trending_keywords` | Get trending keywords for a region |
| `create_report` | Create an async analytics report |
| `get_report` | Get the status or download an async report |

## Usage Examples

### Campaign Performance

```
"How are my Pinterest ad campaigns performing this month?"
```

### Shopping Analytics

```
"Which products are getting the most saves from Pinterest?"
```

### Pin Performance

```
"Show me my top performing pins by engagement"
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
- **Trending discovery** - Find trending products

### For Lifestyle Brands
- **Inspiration tracking** - See how content inspires
- **Board analytics** - Understand collections
- **Seasonal trends** - Capitalize on Pinterest trends

### For Agencies
- **Multi-account management** - Handle client accounts
- **Async reporting** - Generate detailed reports
- **Cross-platform comparison** - Pinterest vs other channels

## Security & Privacy

- **Pinterest Marketing Partner** - Official API access
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

- [Documentation](https://insightfulpipe.com/docs/pinterest-ads)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blogs)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.
