# removeBG (v1.0)

Remove background or replace with solid color

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Source image URL |
| `maskType` | string | Yes | Region to preserve. autoSubjectSegment: preserve foreground subject, remove/replace background; custom: use customMaskUrl; `autoSubjectSegment`, `custom` |
| `backgroundHex` | string | No | Hex color for the new background, e.g. '#ffffff'. Provide at least one of backgroundHex or backgroundId; omit both to remove background (transparent) |
| `backgroundId` | integer | No | Preset background color ID. Run GET /openapi/v1/agent/info to list available IDs. Provide at least one of backgroundHex or backgroundId; omit both to remove background (transparent) |
| `customMaskUrl` | string | No | PNG mask image URL defining the protected region. Required when maskType=custom |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
