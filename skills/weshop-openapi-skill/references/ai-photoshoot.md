# ai-photoshoot (v1.0)

Professional photoshoot by combining a character photo and a reference scene

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Two image URLs: image 1 = character/person, image 2 = reference scene |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Two image URLs: image 1 = character/person, image 2 = reference scene; up to 2 |
| `modelName` | string | No | Model: qwen (default), firered, or nano (supports --image-size); `qwen`, `firered`, `nano`; default `qwen` |
| `textDescription` | string | No | Additional instructions for how the person should appear in the scene |
| `aspectRatio` | string | No | Output aspect ratio (nano also supports 21:9); `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `auto` |
| `imageSize` | string | No | Output resolution (nano model only); `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
