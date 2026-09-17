# gpt-image (v1.0)

High-quality image generation and editing with GPT Image 2 (default), GPT Image 2.5 Flare, or GPT Image 2.5 Sunburst. Select the model with params.modelName; agent/version remain gpt-image/v1.0.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (optional): up to 5 for GPT Image 2; up to 16 for GPT Image 2.5 |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (optional): up to 5 for GPT Image 2; up to 16 for GPT Image 2.5; up to 16 |
| `textDescription` | string | Yes | Describe the image to generate or how to edit reference images |
| `aspectRatio` | string | Yes | Output aspect ratio; 4:5 and 5:4 are only supported by GPT Image 2.5; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`, `4:5`, `5:4`; default `3:4` |
| `imageSize` | string | Yes | Output resolution; `1K`, `2K`, `4K`; default `1K` |
| `quality` | string | Yes | Output quality: low, medium, high for all models; xhigh and max only for GPT Image 2.5; `low`, `medium`, `high`, `xhigh`, `max`; default `low` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
| `modelName` | string | No | Model to use; omitted defaults to GPT Image 2; `gpt-image-2`, `gpt-image-2.5-flare`, `gpt-image-2.5-sunburst`; default `gpt-image-2` |
