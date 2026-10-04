---
name: workato-create-and-retrieve-skill
description: Create a new skill and retrieve its details, then list all skills.
api: openapi/workato-skills-api-openapi.yml
operations:
- createSkill
- getSkill
- listSkills
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/workato-skills-api-openapi.yml ; every operationId checked against the contract
---

# workato-create-and-retrieve-skill

Create a new skill and retrieve its details, then list all skills.

## Steps

1. 1. Use `createSkill` with the request body fields required for a skill (e.g., `name`, `description`, `type`, etc.) as defined in the contract.
2. 2. Use `getSkill` with the path parameter `id` returned from `createSkill` to fetch the newly created skill.
3. 3. Use `listSkills` to retrieve the collection of all skills.

## Rules

- Include an `Authorization: Bearer <token>` header for all requests (bearerAuth).
- No rate limit is defined; on exhaustion the API returns no specific HTTP status.
