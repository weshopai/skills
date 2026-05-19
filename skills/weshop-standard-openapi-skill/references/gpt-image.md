# gpt-image (v1.0)

High-quality image generation and editing with GPT Image 2

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 5, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 5, optional); up to 5 |
| `textDescription` | string | Yes | Describe the image to generate or how to edit reference images |
| `aspectRatio` | string | Yes | Output aspect ratio; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `3:4` |
| `imageSize` | string | Yes | Output resolution; `1K`, `2K`, `4K`; default `1K` |
| `quality` | string | Yes | Output quality tier; `low`, `medium`, `high`; default `low` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
