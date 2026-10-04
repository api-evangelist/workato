---
name: workato-publish-and-consume-messages
description: Publish a message to a topic and then consume messages from that topic.
api: openapi/workato-messages-api-openapi.yml
operations:
- publishMessage
- consumeMessages
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/workato-messages-api-openapi.yml ; every operationId checked against the contract
---

# workato-publish-and-consume-messages

Publish a message to a topic and then consume messages from that topic.

## Steps

1. 1. Use `publishMessage` with the required request body fields for the message.
2. 2. Use `consumeMessages` with the required path parameter `topic_id` and any query parameters for consumption.

## Rules

- Auth: Include a Bearer token in the `Authorization` header as defined by the `bearerAuth` scheme.
- Idempotency: Not applicable; the API does not define idempotency keys.
- Pagination: Not applicable; the consume operation returns a single batch of messages.
- Errors: The API does not specify custom error codes; standard HTTP error responses apply.
