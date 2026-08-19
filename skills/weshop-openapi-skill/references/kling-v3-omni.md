# kling-v3-omni (v1.0)

Multimodal Kling 3.0 Omni video generation from text, optional reference images (up to 4), and an optional reference video, with native audio

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (publicly accessible, up to 4, optional). Refer to them in the prompt as image 1, image 2, etc. |
| `input.videos` | array | No | Optional reference video URL (publicly accessible) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (publicly accessible, up to 4, optional). Refer to them in the prompt as image 1, image 2, etc.; up to 4 |
| `videos` | array | No | Optional reference video URL (publicly accessible); up to 1 |
| `textDescription` | string | Yes | Describe the desired video, character action, camera, and audio |
| `modelName` | string | No | Kling 3.0 Omni model; `Kling_V3_Omni`; default `Kling_V3_Omni` |
| `duration` | string | Yes | Video duration; `3s`, `4s`, `5s`, `6s`, `7s`, `8s`, `9s`, `10s`, `11s`, `12s`, `13s`, `14s`, `15s`; default `5s` |
| `aspectRatio` | string | No | Output aspect ratio. Hidden in the UI when a reference video is provided.; `16:9`, `9:16`, `1:1`; default `16:9` |
| `generateAudio` | string | No | Generate native audio; `true`, `false`; default `false` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
