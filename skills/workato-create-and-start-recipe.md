---
name: workato-create-and-start-recipe
description: Create a new recipe and immediately start it.
api: openapi/workato-recipes-api-openapi.yml
operations:
- createRecipe
- startRecipe
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/workato-recipes-api-openapi.yml ; every operationId checked against the contract
---

# workato-create-and-start-recipe

Create a new recipe and immediately start it.

## Steps

1. 1. `createRecipe` – provide the required request body fields for the new recipe (e.g., name, trigger, actions).
2. 2. `startRecipe` – supply the `id` path parameter returned from `createRecipe` to start the recipe.

## Rules

- Auth: Include a Bearer token in the `Authorization` header as defined by the `bearerAuth` scheme.
- Idempotency: Not applicable; the operations do not define idempotency keys.
