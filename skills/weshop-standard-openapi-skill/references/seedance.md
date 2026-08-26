# seedance (v1.0)

Cinematic AI video generation using Seedance by ByteDance. Seedance_20 remains the default; Seedance_20_Mini is an additive model option.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input / reference image URLs (1–9; multi-image best with Seedance_20 and Seedance_20_Mini) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input / reference image URLs (1–9; multi-image best with Seedance_20 and Seedance_20_Mini); up to 9 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `modelName` | string | No | Seedance model version. Optional — omit or keep Seedance_20 for historical CLI clients; Seedance_20_Mini is additive; `Seedance_20`, `Seedance_20_Mini`, `Seedance_10_Pro`, `Seedance_10_Pro_Fast`; default `Seedance_20` |
| `duration` | string | No | Video duration (Seedance_20/20_Mini: 4s-15s; 1.0_Pro/Fast: 2s-12s); default `4s` |
| `aspectRatio` | string | No | Output aspect ratio. 21:9 is supported on Seedance_20 and Seedance_20_Mini; `21:9`, `16:9`, `9:16`, `3:4`, `4:3`, `1:1`; default `3:4` |
| `generateAudio` | string | No | Generate audio (Seedance_20 and Seedance_20_Mini only); `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
