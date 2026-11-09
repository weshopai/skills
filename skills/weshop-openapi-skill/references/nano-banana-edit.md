# nano-banana-edit (v1.0)

Image generation and editing with Nano Banana / Pro / 2 / 2.1. Select nano2.1 explicitly; CLI default remains nano2, imageSize 1K, aspectRatio auto.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 9, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 9, optional); up to 9 |
| `textDescription` | string | No | Describe the desired edit or generation (optional; image-only edits supported) |
| `modelName` | string | Yes | Model variant: nano1 (Nano Banana), nano (Pro), nano2 (2, unchanged default), nano2.1 (2.1); `nano1`, `nano`, `nano2`, `nano2.1`; default `nano2` |
| `aspectRatio` | string | Yes | Output aspect ratio; panoramic 1:4, 4:1, 1:8, 8:1 are available for nano2 and nano2.1; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `4:5`, `5:4`, `16:9`, `9:16`, `21:9`, `1:4`, `4:1`, `1:8`, `8:1`; default `auto` |
| `imageSize` | string | Yes | Output resolution for nano, nano2 and nano2.1; 1K remains the CLI default; `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
