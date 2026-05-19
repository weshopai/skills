# wan-ai (v1.0)

AI video generation from images and text using Wan AI

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `duration` | string | No | Video duration; `3s`, `4s`, `5s`, `6s`, `7s`, `8s`; default `5s` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
