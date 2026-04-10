# z-image (v1.0)

Text-to-image generation with Z-Image by Alibaba

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `textDescription` | string | Yes | Describe the desired image |
| `aspectRatio` | string | No | Output aspect ratio; `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `1:1` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
