# ai-image-animation (v1.0)

Animate a static image into a dynamic video using Kling

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL to animate |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL to animate; up to 1 |
| `textDescription` | string | Yes | Describe the desired animation or motion |
| `modelName` | string | No | Kling model: Kling_3_0 (default) or Kling_2_6; `Kling_3_0`, `Kling_2_6`; default `Kling_3_0` |
| `duration` | string | No | Video duration (Kling_3_0: 3s-15s; Kling_2_6: 5s, 10s); default `5s` |
| `generateAudio` | string | No | Generate audio; `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
