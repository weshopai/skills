# aiproduct (v1.0)

Product still-life generation and product background editing

**Tips:** Use `locationId` for best results (run `GET /openapi/v1/agent/info` to list available IDs). If using only `textDescription` without a preset ID, set `generatedContent` to `freeCreation`.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Source image URL |
| `generatedContent` | string | Yes | Generation mode: freeCreation (free AI) or referToOrigin (stay close to source); `freeCreation`, `referToOrigin` |
| `maskType` | string | Yes | Region to preserve. autoSubjectSegment: preserve the product, replace background; custom: use customMaskUrl; `autoSubjectSegment`, `custom` |
| `textDescription` | string | No | Describe the desired background or scene. Provide at least one of locationId or textDescription |
| `locationId` | integer | No | Preset scene ID for background replacement. Run GET /openapi/v1/agent/info to list available IDs. Provide at least one of locationId or textDescription |
| `negTextDescription` | string | No | Elements to avoid in the result |
| `customMaskUrl` | string | No | PNG mask image URL defining the protected region. Required when maskType=custom |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
