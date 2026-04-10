# ai-poster (v1.0)

Create a designed poster from text prompt and optional reference images

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 6, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 6, optional); up to 6 |
| `textDescription` | string | Yes | Describe the desired poster |
| `modelName` | string | No | Model: jimeng (default), nano, or nano2 (nano/nano2 support --image-size and --aspect-ratio); `jimeng`, `nano`, `nano2`; default `jimeng` |
| `aspectRatio` | string | No | Output aspect ratio (nano/nano2 only); `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `9:16`, `16:9`, `21:9`; default `1:1` |
| `imageSize` | string | No | Output resolution (nano/nano2 only); `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
