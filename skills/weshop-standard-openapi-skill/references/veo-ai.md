# veo-ai (v1.0)

Cinematic AI video generation with Google Veo 3.1

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `modelName` | string | Yes | Veo model version; `Veo_3_1`, `Veo_3_1_Fast`; default `Veo_3_1` |
| `aspectRatio` | string | Yes | Output aspect ratio (Veo_3_1 default 16:9; Veo_3_1_Fast default 9:16); `16:9`, `9:16`; default `16:9` |
| `duration` | string | Yes | Video duration; `4s`, `6s`, `8s`; default `4s` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
