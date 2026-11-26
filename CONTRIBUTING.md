# Maintaining this plugin

`skills/` is generated from the DesignMD Pro monorepo (`apps/web/mcp-skills/`, bundled with shared files and the generated font table by `apps/web/scripts/build-mcp-skills.ts`). They are the same skills `/mcp` serves over `skill://designmdpro/…`. Do not edit them here. Change them in the monorepo, then re-export them.

Before every release:

1. Bump `version` in `plugin.json`.
2. Run `agy plugin validate --strict .`
