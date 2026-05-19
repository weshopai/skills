# grok-imagine (v1.0)

High-resolution image generation using xAI Aurora (Grok Imagine)

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URL (optional); up to 1 |
| `textDescription` | string | Yes | Describe the desired image |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
