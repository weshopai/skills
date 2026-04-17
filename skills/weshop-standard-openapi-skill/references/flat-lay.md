# flat-lay (v1.0)

Create professional flat-lay product images from a photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input garment or model photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input garment or model photo URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired flat-lay output |
| `modelName` | string | No | Model: nano2 (default) or nano; `nano2`, `nano`; default `nano2` |
| `imageSize` | string | No | Output resolution; `1K`, `2K`, `4K`; default `1K` |
| `aspectRatio` | string | No | Output aspect ratio; `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `9:16`, `16:9`, `21:9`; default `1:1` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
