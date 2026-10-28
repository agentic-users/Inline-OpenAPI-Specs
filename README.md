# Inline OpenAPI Specs

A library of OpenAPI descriptions for use with Inline's **Add a REST API** feature. Each folder holds one API's spec (YAML and JSON).

## Available APIs

| API | Version | Methods | Files |
|---|---|---|---|
| Slack Web API | built 2026-10-12 | 340 | [`slack/openapi.yaml`](slack/openapi.yaml), [`slack/openapi.json`](slack/openapi.json) |
| Airtable Web API | built 2026-10-12 | 51 operations | [`airtable/openapi.yaml`](airtable/openapi.yaml), [`airtable/openapi.json`](airtable/openapi.json) |
| Todoist REST API v2 | built 2026-10-12 | 33 operations | [`todoist/openapi.yaml`](todoist/openapi.yaml), [`todoist/openapi.json`](todoist/openapi.json) |
| Higgsfield API | unofficial copy | 50 operations | [`higgsfield/openapi.yaml`](higgsfield/openapi.yaml), [`higgsfield/openapi.json`](higgsfield/openapi.json) |
| Gemini API | built 2026-10-22 | 78 operations, tagged by AI Studio category | [`gemini/openapi.yaml`](gemini/openapi.yaml), [`gemini/openapi.json`](gemini/openapi.json) |

## Loading a spec into Inline

Paste a raw file URL into **Add a REST API → From an address**, for example:

```
https://raw.githubusercontent.com/agentic-users/Inline-OpenAPI-Specs/main/slack/openapi.json
```

## Notes on the Slack spec

- **Not published by Slack.** This is a community-built description based on the public documentation at docs.slack.dev. It is not affiliated with, endorsed by, or supported by Slack.
- **Built from summarized documentation.** Parameters, scopes, and error codes come from summaries of each method page. Fields the docs did not state a type for are marked "type not stated on docs page" and have no type.
- **Not tested against the live API.** Verify behavior against Slack's documentation before relying on it in production.
- Slack and its trademarks belong to their owners. Slack's API terms apply to your use of the Slack API itself.

## Gemini notes

Unofficial, built from Google's API reference (ai.google.dev/api) plus the googleapis proto files for content types, and untested against the live API. The Live and Live Music APIs are WebSocket-based and are not included. Auth is an API key in the `x-goog-api-key` header.
