# face-forge (v1.0)

AI face morph, face swap, and portrait generation

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 3, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 3, optional); up to 3 |
| `textDescription` | string | No | Describe the desired portrait or transformation; default `Please generate a realistic portrait photograph of an Asian woman with long black hair, wearing a pure white sleeveless outfit, set against a plain white background.` |
| `modelName` | string | No | Model: jimeng (default, no image-size/aspect-ratio) or nano (supports image-size and aspect-ratio); `jimeng`, `nano`; default `jimeng` |
| `imageSize` | string | No | Output resolution (nano model only); `1K`, `2K`, `4K`; default `1K` |
| `aspectRatio` | string | No | Output aspect ratio (nano model only); `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `9:16`, `16:9`, `21:9`; default `1:1` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
