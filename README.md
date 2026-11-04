# PayBridge System Design

Keep remittance orchestration separate from ledger journals and use stable references to reconcile simulated payout attempts.

This repository documents the architecture of the [reviewed implementation](https://github.com/Danny-Kyle/paybridge/tree/0b14f948a492735100752bfb44aceb1fd78421cc).

## Decision dossier

- [PDF](dossier/Architecture%20decision%20dossier.pdf)
- [Editable Word version](dossier/Architecture%20decision%20dossier.docx)

## C4 diagrams

- [C4 context](diagrams/c4-context.drawio)
- [C4 container](diagrams/c4-container.drawio)
- [C4 component-remittance-path](diagrams/c4-component-remittance-path.drawio)

Open the editable files with [diagrams.net](https://app.diagrams.net/).

## API contract

The [OpenAPI 3.0.3 contract](api/openapi-paybridge-remittance-workflow.json) covers the workflow described in the dossier. Validate it with `npx @redocly/cli lint --extends minimal api/openapi-paybridge-remittance-workflow.json`.

## AI usage

See the [AI log](ai/ai-log.md) for the source checks behind these artifacts.
