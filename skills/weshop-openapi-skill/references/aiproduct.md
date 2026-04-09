# aiproduct (v1.0)

Product scene generation and product background editing.

**Tips:** Use `locationId` for best results (run `GET /openapi/v1/agent/info` to list available IDs). If using only `textDescription` without preset IDs, set `generatedContent` to `freeCreation`.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Publicly reachable source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `generatedContent` | string | Yes | `freeCreation` or `referToOrigin` |
| `maskType` | string | Yes | Supports `autoSubjectSegment` and `custom` |
| `locationId` | int | Conditional | Replace background with this scene ID. Provide at least one of `locationId` or `textDescription` |
| `textDescription` | string | Conditional | Describe the desired result. Provide at least one of `locationId` or `textDescription` |
| `negTextDescription` | string | No | Elements you do not want in the result |
| `customMask` | string(base64) | Conditional | Required for `maskType=custom` when URL absent |
| `customMaskUrl` | string(url) | Conditional | Required for `maskType=custom` when base64 absent |
| `batchCount` | int | No | Range `1-16`, default `4` |
