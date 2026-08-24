# seedream (v1.0)

AI image generation and editing with Seedream 5.0 Pro or Lite by ByteDance. modelName is optional for historical CLI/OpenAPI clients.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (Seedream_50_Pro: up to 10; Seedream_50_Lite: up to 14; optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (Seedream_50_Pro: up to 10; Seedream_50_Lite: up to 14; optional); up to 14 |
| `textDescription` | string | Yes | Describe the desired image or edit |
| `modelName` | string | No | Seedream model. Optional — omit to keep historical CLI/OpenAPI payloads working; backend then defaults to Seedream_50_Pro; `Seedream_50_Pro`, `Seedream_50_Lite`; default `Seedream_50_Pro` |
| `imageSize` | string | No | Output resolution. Seedream_50_Pro: 1K (default), 2K. Seedream_50_Lite: 2K (default), 3K. 3K is Lite-only; `1K`, `2K`, `3K` |
| `aspectRatio` | string | No | Output aspect ratio. Seedream_50_Pro default: auto. Seedream_50_Lite default: 3:4. auto is Pro-oriented (adapts to the first reference image); `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9` |
| `outputFormat` | string | No | Output format; `jpeg`, `png`; default `jpeg` |
| `tools` | array | No | Enable tools, e.g. web_search (Seedream_50_Lite only; not supported on Pro) |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
