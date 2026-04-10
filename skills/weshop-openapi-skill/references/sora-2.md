# sora-2 (v1.0)

Cinematic video generation with realistic physics using OpenAI Sora 2

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `duration` | string | No | Video duration; `4s`, `8s`, `12s`; default `4s` |
| `aspectRatio` | string | No | Output aspect ratio; `16:9`, `9:16`; default `16:9` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
