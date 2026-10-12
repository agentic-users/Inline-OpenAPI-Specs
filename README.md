# Inline OpenAPI Specs

A library of OpenAPI descriptions for use with Inline's **Add a REST API** feature. Each folder holds one API's spec, in YAML and JSON.

## Available APIs

| API | Version | Methods | Files |
|---|---|---|---|
| Slack Web API | built 2026-10-12 | 340 | [`slack/openapi.yaml`](slack/openapi.yaml), [`slack/openapi.json`](slack/openapi.json) |

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
