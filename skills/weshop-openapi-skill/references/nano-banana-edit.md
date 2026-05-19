# nano-banana-edit (v1.0)

Image generation and editing with Nano Banana / Pro / Nano Banana 2 models

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 9, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 9, optional); up to 9 |
| `textDescription` | string | No | Describe the desired edit or generation (optional; image-only edits supported) |
| `modelName` | string | Yes | Model variant: nano1 (Nano Banana), nano (Nano Banana Pro), nano2 (Nano Banana 2); `nano1`, `nano`, `nano2`; default `nano2` |
| `aspectRatio` | string | Yes | Output aspect ratio; 1:4, 4:1, 1:8, 8:1 are only available when modelName is nano2; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `4:5`, `5:4`, `16:9`, `9:16`, `21:9`, `1:4`, `4:1`, `1:8`, `8:1`; default `auto` |
| `imageSize` | string | Yes | Output resolution (used for nano / nano2; ignored for nano1 in the product UI but still accepted by the API); `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
