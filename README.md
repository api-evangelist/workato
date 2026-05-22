# Workato (workato)

Workato is an enterprise automation and integration platform that enables organizations to integrate their apps and automate business workflows without extensive coding. The platform now layers Enterprise MCP, Workato Genies AI agents, Agent Studio, and Workato Embedded on top of its iPaaS foundation, with API Edge Gateway for on-premises deployment and RBAC 2.0 with environment- and project-scoped roles. Workato has been recognized as an 8x Leader and 3x Furthest in Vision in the 2026 Gartner Magic Quadrant for Integration Platform as a Service.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

API Management, Agentic, Automation, B2B, Embedded iPaaS, Enterprise, Integration, Orchestration, Workflow, iPaaS

## Timestamps

- **Created:** 2025-06-05
- **Modified:** 2026-05-22

## APIs

### Workato Developer API
Cloud-based platform for automation, integration, and AI orchestration with resources for managing recipes, connections, jobs, connectors, API platform, custom OAuth profiles, data tables, tag assignments, custom connectors, recipe lifecycle management, and the Agent Studio, MCP Server, Event Streams, and Test Automation surfaces. Bearer token auth via API clients (legacy API keys deprecated July 14, 2025). Regional base URLs across US, EU, JP, SG, AU, IL, CN, KR, and the developer sandbox.

**Human URL:** [https://www.workato.com/](https://www.workato.com/)

#### Tags: Embedded SaaS Integration, Orchestration, Agentic, iPaaS

#### Key Properties
- [Workato API Docs](https://docs.workato.com/workato-api.html)
- [Authentication](https://docs.workato.com/workato-api/authentication.html)
- [Rate Limiting](https://docs.workato.com/workato-api/rate-limiting.html)
- [Connector SDK](https://github.com/workato/workato-connector-sdk)
- [Developer API OpenAPI](openapi/workato-developer-api-openapi.yml)
- [Agent Studio OpenAPI](openapi/workato-agent-studio-openapi.yml)

### Workato Embedded Partner API
Endpoints for partners to programmatically create and manage customers, recipes, connections, environments (Development, Test, Production), customer properties, jobs, team members, and the embedded API platform within the Workato Embedded platform.

**Human URL:** [https://docs.workato.com/oem/oem-api.html](https://docs.workato.com/oem/oem-api.html)

#### Tags: Embedded iPaaS, OEM, Partner API

### Workato Event Streams Public API
HTTP-based publish and consume for event topics — single publish, batch publish of up to 100 messages, and consumption with long polling. Rate limited to 60 requests per minute with a 1 MB maximum payload.

**Human URL:** [https://docs.workato.com/workato-api/pubsub.html](https://docs.workato.com/workato-api/pubsub.html)

#### Tags: Event Streams, Messaging, Pub/Sub, REST

### Workato MCP Server API
Programmatic management of Model Context Protocol servers that expose Workato API collections as tools for AI agents. Supports server creation, tool management, user group assignment, and policy configuration. MCP servers generate unique authenticated URLs usable by Claude Desktop and Cursor. Workato now markets this as Enterprise MCP, with nine prebuilt servers including Dropbox, Freshdesk, ZoomInfo, Notion, Discord, and Microsoft Teams. Available in US, EU, AU, JP, and SG data centers.

**Human URL:** [https://docs.workato.com/mcp.html](https://docs.workato.com/mcp.html)

#### Tags: AI Agents, MCP, Model Context Protocol, REST

## Common Properties

- [GitHub Organization](https://github.com/workato) — 67 public repositories
- [Pricing](https://www.workato.com/pricing) — contact-sales / quote-based
- [Security](https://www.workato.com/platform/security)
- [Trust Center](https://trust.workato.com/)
- [Status Page](https://status.workato.com/) — Atlassian Statuspage
- [Blog](https://www.workato.com/the-connector/)
- [Changelog](https://www.workato.com/product-hub/changelog/)
- [What's New](https://www.workato.com/product-hub/whats-new/)
- [Developer Portal](https://docs.workato.com/)
- [Community](https://community.workato.com/)
- [Support](https://support.workato.com/)
- [Academy](https://academy.workato.com/)
- [Certification](https://www.workato.com/certification)
- [Partners](https://partners.workato.com/)
- [Events](https://www.workato.com/events)
- [API Management](https://docs.workato.com/api-management.html)
- [Connector Catalog](https://app.workato.com/browse/recipes)

## Artifacts

Machine-readable API specifications and supporting artifacts.

### OpenAPI

- [Workato Developer API](openapi/workato-developer-api-openapi.yml)
- [Workato Agent Studio API](openapi/workato-agent-studio-openapi.yml)
- [Workato Event Streams Public API](openapi/workato-event-streams-openapi.yml)
- [Workato MCP Server API](openapi/workato-mcp-server-openapi.yml)

### AsyncAPI

- [Workato Event Streams](asyncapi/workato-event-streams-asyncapi.yml)

### JSON Schema (25 files)

Schemas under [`json-schema/`](json-schema/) cover Agent Studio (Genie, Knowledge Base, Skill, Data Source, User Group), Developer API (Recipe, Recipe Version, Data Table, Data Table Column), Event Streams (Message, batch publish, consume), MCP Server (MCP Server, Tool, Policy, User Group), and the top-level Recipe and Genie entities.

### JSON Structure (25 files)

Parallel structure definitions under [`json-structure/`](json-structure/) for the same entities.

### JSON-LD

- [Workato Context](json-ld/workato-context.jsonld)

### Examples (26 files)

Request and response payload examples under [`examples/`](examples/) covering all four API surfaces.

## Capabilities

Naftiko capabilities under [`capabilities/`](capabilities/) — ten per-resource capability definitions across the four API surfaces:

- [agent-studio-genies.yaml](capabilities/agent-studio-genies.yaml)
- [agent-studio-knowledge-bases.yaml](capabilities/agent-studio-knowledge-bases.yaml)
- [agent-studio-skills.yaml](capabilities/agent-studio-skills.yaml)
- [developer-recipes.yaml](capabilities/developer-recipes.yaml)
- [developer-data-tables.yaml](capabilities/developer-data-tables.yaml)
- [event-streams-messages.yaml](capabilities/event-streams-messages.yaml)
- [mcp-server-mcp-servers.yaml](capabilities/mcp-server-mcp-servers.yaml)
- [mcp-server-tools.yaml](capabilities/mcp-server-tools.yaml)
- [mcp-server-policies.yaml](capabilities/mcp-server-policies.yaml)
- [mcp-server-user-groups.yaml](capabilities/mcp-server-user-groups.yaml)

## Rules

- [Workato Spectral Rules](rules/workato-spectral-rules.yml) — Spectral ruleset enforcing Workato API conventions.

## Vocabulary

- [Workato Vocabulary](vocabulary/workato-vocabulary.yml) — unified taxonomy across operational (OpenAPI) and capability (Naftiko) dimensions.

## Commercial

- [Plans & Pricing](plans/workato-plans-pricing.yml) — API Commons Plans 0.1 capturing Workato's custom subscription pricing structured around recipes + tasks + connectors + seats.
- [Rate Limits](rate-limits/workato-rate-limits.yml) — API Commons Rate Limits 0.1 covering Developer, Embedded, and Event Streams Public API limits.
- [FinOps](finops/workato-finops.yml) — FinOps Framework / FOCUS-aligned billing meters for tasks, recipes, HVRs, seats, and premium connectors.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
