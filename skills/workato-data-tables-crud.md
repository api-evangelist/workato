---
name: workato-data-tables-crud
description: Create, retrieve, update, and delete a data table in Workato.
api: openapi/workato-data-tables-api-openapi.yml
operations:
- createDataTable
- getDataTable
- updateDataTable
- deleteDataTable
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/workato-data-tables-api-openapi.yml ; every operationId checked against the contract
---

# workato-data-tables-crud

Create, retrieve, update, and delete a data table in Workato.

## Steps

1. 1. Use `createDataTable` with the request body fields required to define the new data table.
2. 2. Use `getDataTable` with the path parameter `data_table_id` returned from step 1 to retrieve the table details.
3. 3. Use `updateDataTable` with the path parameter `data_table_id` and the request body fields to modify the table.
4. 4. Use `deleteDataTable` with the path parameter `data_table_id` to remove the table.

## Rules

- Auth: Include a Bearer token in the `Authorization` header (`Bearer <token>`).
- Idempotency: The `createDataTable` operation is not idempotent; repeat calls will create duplicate tables.
- Pagination: Not applicable; list operations are not used in this task.
- Errors: The API returns standard HTTP error codes; no specific error handling is documented.
