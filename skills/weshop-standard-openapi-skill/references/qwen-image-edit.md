# qwen-image-edit (v1.0)

AI image editing and generation with natural language using Qwen

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 5, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 5, optional); up to 5 |
| `textDescription` | string | Yes | Describe the desired edit or generation |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
