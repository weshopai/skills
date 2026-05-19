# happyhorse (v1.0)

Cinematic AI video generation with HappyHorse 1.0

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `modelName` | string | Yes | HappyHorse model version; `HappyHorse_10`; default `HappyHorse_10` |
| `aspectRatio` | string | Yes | Output aspect ratio; `9:16`, `16:9`, `3:4`, `4:3`, `1:1`; default `9:16` |
| `duration` | string | Yes | Video duration; `3s`, `4s`, `5s`, `6s`, `7s`, `8s`, `9s`, `10s`, `11s`, `12s`, `13s`, `14s`, `15s`; default `3s` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
