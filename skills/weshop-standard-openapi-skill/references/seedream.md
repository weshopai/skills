# seedream (v1.0)

AI image generation and editing with Seedream 5.0 by ByteDance

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 14, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 14, optional); up to 14 |
| `textDescription` | string | Yes | Describe the desired image or edit |
| `imageSize` | string | No | Output resolution; `2K`, `3K`; default `2K` |
| `aspectRatio` | string | No | Output aspect ratio; `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `3:4` |
| `outputFormat` | string | No | Output format; `jpeg`, `png`; default `jpeg` |
| `tools` | array | No | Enable tools, e.g. web_search |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
