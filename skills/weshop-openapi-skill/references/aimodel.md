# aimodel (v1.0)

Fashion model generation or model-scene editing.

**Tips:** Use `locationId` / `fashionModelId` for best results (run `GET /openapi/v1/agent/info` to list available IDs). If using only `textDescription` without preset IDs, set `generatedContent` to `freeCreation`.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Publicly reachable source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `generatedContent` | string | Yes | `freeCreation` or `referToOrigin` |
| `maskType` | string | Yes | Supports `autoApparelSegment`, `autoUpperApparelSegment`, `autoLowerApparelSegment`, `autoSubjectSegment`, `autoHumanSegment`, `inverseAutoHumanSegment`, `custom` |
| `locationId` | int | Conditional | Replace background with this scene ID. Provide at least one of `locationId`, `fashionModelId`, or `textDescription` |
| `fashionModelId` | int | Conditional | Replace model face with this fashion model. Provide at least one of `locationId`, `fashionModelId`, or `textDescription` |
| `textDescription` | string | Conditional | Describe the desired result. Provide at least one of `locationId`, `fashionModelId`, or `textDescription` |
| `negTextDescription` | string | No | Elements you do not want in the result |
| `customMask` | string(base64) | Conditional | Required when `maskType=custom` and `customMaskUrl` absent |
| `customMaskUrl` | string(url) | Conditional | Required when `maskType=custom` and `customMask` absent |
| `batchCount` | int | No | Range `1-16`, default `4` |
| `pose` | string | No | `originalImagePose` (default): keep source pose. `referenceImagePose`: adopt pose from `locationId` reference. `freePose`: AI decides freely |
