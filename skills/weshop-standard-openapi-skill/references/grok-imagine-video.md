# grok-imagine-video (v1.0)

Cinematic AI video generation with native audio using xAI Grok Imagine

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `duration` | string | No | Video duration; `6s`, `10s`; default `6s` |
| `aspectRatio` | string | No | Output aspect ratio; `16:9`, `9:16`, `1:1`; default `16:9` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
