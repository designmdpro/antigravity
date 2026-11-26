# DesignMD Pro for Antigravity

Restyle your project after a real website. [DesignMD Pro](https://www.designmdpro.app) is a curated library of website design systems published as `DESIGN.md` files ([google-labs-code/design.md](https://github.com/google-labs-code/design.md) spec), with revision history. This plugin connects Antigravity to that library and adds two skills that turn a reference site or a loose brief into changes to your theme.

## What's included

### MCP server

The remote DesignMD Pro MCP server at `https://www.designmdpro.app/mcp`:

| Tool              | What it does                                                         |
| ----------------- | -------------------------------------------------------------------- |
| `search_websites` | Find websites by name, category, tag or free text                    |
| `list_categories` | List valid category filters                                          |
| `list_tags`       | List valid tag filters                                               |
| `get_design_md`   | Read a website's `DESIGN.md`: tokens, guidelines, only the sections you ask for |
| `list_revisions`  | List the revision history of a website's design system               |

### Skills

- **`/restyle-from-reference`**: "make it look like Linear". Finds the site, reads its tokens, maps them onto your project's theme layer, applies them, then audits the codebase for leftovers of the old design.
- **`/design-direction-explorer`**: "make it feel calmer". Turns a loose brief into concrete directions backed by real websites, shows them as palette cards to choose from, then restyles the project once you confirm.

## Access

The plugin works without an account: search and public design systems are available anonymously, with rate limits.

[DesignMD Pro](https://www.designmdpro.app/pricing) subscribers get full tokens for Pro websites and their revision history. Sign in when Antigravity asks for it, which goes through the standard OAuth 2.1 flow in your browser. Access follows your current plan.

## Install

Install **DesignMD Pro** from the Antigravity Marketplace, or from this repository:

```sh
agy plugin install https://github.com/designmdpro/antigravity
```

## Try it

- Make this app look like Linear
- Show me three calmer, more premium design directions for this project
- Find fintech websites with dark themes and compare their color tokens

## Security

`DESIGN.md` content is extracted from third-party websites. The skills treat it as data, never as instructions.

## Links

- Website: https://www.designmdpro.app
- MCP docs: https://www.designmdpro.app/integrations/mcp
- CLI: `npx designmdpro`
