# vidu-ai (v1.0)

Cinematic AI video generation with Vidu Q3 Pro models

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `modelName` | string | Yes | Vidu model version; `Vidu_Q3_Pro`, `Vidu_Q3_Pro_Fast`; default `Vidu_Q3_Pro` |
| `aspectRatio` | string | Yes | Output aspect ratio (Vidu_Q3_Pro default 16:9; Vidu_Q3_Pro_Fast default 9:16); `16:9`, `9:16`, `3:4`, `4:3`, `1:1`; default `16:9` |
| `duration` | string | Yes | Video duration from 4s through 16s; default `4s` |
| `generateAudio` | string | Yes | Generate audio track; `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
