# seedance (v1.0)

Cinematic AI video generation using Seedance by ByteDance

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `modelName` | string | No | Seedance model version; `Seedance_20`, `Seedance_15_Pro`, `Seedance_10_Pro`, `Seedance_10_Pro_Fast`; default `Seedance_20` |
| `duration` | string | No | Video duration (Seedance_20/1.5_Pro: 4s-15s; 1.0_Pro/Fast: 2s-12s); default `4s` |
| `aspectRatio` | string | No | Output aspect ratio; `21:9`, `16:9`, `9:16`, `3:4`, `4:3`, `1:1`; default `3:4` |
| `generateAudio` | string | No | Generate audio (Seedance_20 and 1.5_Pro only); `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
