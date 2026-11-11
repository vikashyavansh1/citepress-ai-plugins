# CitePress for AI apps

Plugins and registry entries for **CitePress CRM** and **CitePress CMS**. The tools live on our MCP
servers, so new tools and fixes arrive without updating anything here.

| Folder | What it is |
|---|---|
| `citepress-crm/` | CitePress CRM (`https://crm.citepress.org/api/mcp`) with workflow skills and a rule. A Claude plugin (`.claude-plugin/`) and a Cursor plugin (`.cursor-plugin/`) in one folder. |
| `citepress-cms/` | Your own CitePress site's MCP (`https://<your-site>/api/mcp`). Asks for the site's address. |
| `registry/` | `server.json` for the official MCP Registry (`org.citepress/crm`, `org.citepress/cms`). |

## Install

Claude Code:

```
/plugin marketplace add vikashyavansh1/citepress-ai-plugins
/plugin install citepress-crm@citepress
```

Cursor: install from the Cursor Marketplace, or add the MCP server directly:
`cursor://anysphere.cursor-deeplink/mcp/install?name=citepress-crm&config=eyJ1cmwiOiJodHRwczovL2NybS5jaXRlcHJlc3Mub3JnL2FwaS9tY3AifQ==`

Any other MCP client: add `https://crm.citepress.org/api/mcp` (CRM) or `https://<your-site>/api/mcp`
(CMS) as a remote server. Sign-in happens in your browser.

Help: https://crm.citepress.org/integrations/ai · Support: vikash@buldrr.com · Security reports: see `SECURITY.md`.
