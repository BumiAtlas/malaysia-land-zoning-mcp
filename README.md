# Malaysia Land Lots & Local Plan Zoning MCP

Connect your AI assistant to [BumiAtlas](https://bumiatlas.com) for Malaysian land research through the Model Context Protocol.

This listing is a focused entry point for:

- Cadastral land lots from JUPEM's National Digital Cadastral Database (NDCDB): UPI, state, district, mukim, section, lot number, area and boundary
- Lot lookup by UPI, by lot number ("Lot 3193", "PT 1234") narrowed to a state, district, mukim or section, or by coordinates
- Local-plan land-use zoning (Rancangan Tempatan) from PLANMalaysia at any point: land use, land-use code, plan status (existing, committed, proposed), plan and local authority
- The zoning over a lot, with each zone's share of it
- Satellite and street map images of a lot and its neighbours, labelled by lot number

Coverage grows state by state: lots and zoning are loaded for some states so far, and zoning covers more states than lots.


## Connect

```
https://bumiatlas.com/mcp/malaysia
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/malaysia](https://bumiatlas.com/mcp-docs/malaysia).

## Tools

| Tool | Description |
|---|---|
| `MY_lot_search` | Find lots by UPI, lot number with state/district/mukim/section codes, or `latitude, longitude` |
| `MY_lot_get` | One lot: state, district, mukim, section, area and the local-plan zones covering it; boundary as GeoJSON |
| `MY_lot_image` | Satellite or street map image of a lot or point, with every lot in view outlined and labelled with its lot number |
| `MY_zoning_get` | Local-plan zone at a point or by id: land use (Malay and English), code, status, plan, local authority |

## Example prompts

- *"Look up UPI 1601400113193: how big is the lot and what is it zoned for?"*
- *"Which lot is at 1.7156, 103.4852 in Johor?"*
- *"Is this land zoned for housing or agriculture in the local plan?"*
- *"Is the zoning here existing, committed or only proposed?"*

## Data sources

Lots from JUPEM (Jabatan Ukur dan Pemetaan Malaysia), National Digital Cadastral Database. Zoning from PLANMalaysia local plans (gtzoning). Lots have no owner, title or tenure information.
