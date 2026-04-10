# aimodel (v1.0)

Apparel model photos, model replacement, scene replacement

**Tips:** Use `locationId` / `fashionModelId` for best results (run `GET /openapi/v1/agent/info` to list available IDs). If using only `textDescription` without preset IDs, set `generatedContent` to `freeCreation`.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Source image URL |
| `generatedContent` | string | Yes | Generation mode: freeCreation (free AI) or referToOrigin (stay close to source); `freeCreation`, `referToOrigin` |
| `maskType` | string | Yes | Region to preserve. autoApparelSegment: full-body clothing; autoUpperApparelSegment: upper garment only; autoLowerApparelSegment: lower garment only; autoSubjectSegment: foreground subject; autoHumanSegment: body + background (replace face); inverseAutoHumanSegment: face only (replace outfit + background); custom: use customMaskUrl; `autoApparelSegment`, `autoUpperApparelSegment`, `autoLowerApparelSegment`, `autoSubjectSegment`, `autoHumanSegment`, `inverseAutoHumanSegment`, `custom` |
| `textDescription` | string | No | Describe the desired look, style, or scene. Provide at least one of locationId, fashionModelId, or textDescription |
| `locationId` | integer | No | Preset scene ID for background replacement. Run GET /openapi/v1/agent/info to list available IDs. Provide at least one of locationId, fashionModelId, or textDescription |
| `fashionModelId` | integer | No | Preset fashion model ID for model replacement. Run GET /openapi/v1/agent/info to list available IDs. Provide at least one of locationId, fashionModelId, or textDescription |
| `negTextDescription` | string | No | Elements to avoid in the result |
| `pose` | string | No | Pose control. originalImagePose: keep source pose (default); referenceImagePose: adopt pose from locationId reference; freePose: AI decides freely; `originalImagePose`, `referenceImagePose`, `freePose`; default `originalImagePose` |
| `customMaskUrl` | string | No | PNG mask image URL defining the protected region. Required when maskType=custom |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
