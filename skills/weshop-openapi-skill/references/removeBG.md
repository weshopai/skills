# removeBG (v1.0)

Remove background or replace it with a solid color/background preset.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Publicly reachable source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `maskType` | string | Yes | Supports `autoSubjectSegment` and `custom` |
| `backgroundId` | int | Conditional | Replace background with this preset color ID. Provide at least one of `backgroundId` or `backgroundHex` |
| `backgroundHex` | string | Conditional | Replace background with this hex color, e.g. `#ced2ce`. Provide at least one of `backgroundId` or `backgroundHex` |
| `customMask` | string(base64) | Conditional | Required when `maskType=custom` and URL absent |
| `customMaskUrl` | string(url) | Conditional | Required when `maskType=custom` and base64 absent |
| `batchCount` | int | No | Range `1-16`, default `4` |
