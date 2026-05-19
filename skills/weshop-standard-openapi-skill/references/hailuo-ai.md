# hailuo-ai (v1.0)

Cinematic AI video generation with MiniMax Hailuo models

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene or motion |
| `modelName` | string | Yes | Hailuo model version; `Hailuo_02`, `Hailuo_2_3_Fast`, `Hailuo_2_3`; default `Hailuo_02` |
| `duration` | string | Yes | Video duration; `6s`, `10s`; default `6s` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
