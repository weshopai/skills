# firered-image-edit (v1.0)

Image editing and generation with FireRed open-source model

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 3, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 3, optional); up to 3 |
| `textDescription` | string | Yes | Describe the desired edit or generation |
| `aspectRatio` | string | No | Output aspect ratio; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`; default `auto` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
