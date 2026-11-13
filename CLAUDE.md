# wz-where-used — CAP project for Personal



`personal` · `cap` · 2026-11-13. Conventions win: `../../memory/conventions.md` ·
landscape: `../../memory/landscape.md` · project memory: `memory/`.

## Stack
CAP (Node.js/Java) on BTP Cloud Foundry, HANA Cloud / SQLite locally. **TypeScript first**
(cds-typer); check the **CAP MCP** (`mcp__cap__*`) for best practices before every change.
Skills: `sap:cap-cds-modeling`, `sap:hana-hdi`, `sap:btp-platform` · Expert: `sap:cap-developer`.

## Key paths
`db/` model · `srv/` services+handlers (`.ts`) · `app/` UI · `test/` cds.test ·
`mta.yaml` (+`<env>.mtaext`) · `xs-security.json` · `docs/designs`, `docs/plans`

## Checks before "done"
`npx cds compile srv` / `cds build` · `npm test` · `npx eslint .` · browser e2e against the deployed
dev app with the hub's login: `sapctl e2e run <customer> <app> -- npx playwright test` (`sap:landscape-access`)

Dev target: **dev** (settings generated) · logins/prod: `sap:landscape-access`.
