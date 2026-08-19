# sulphur2 (v1.0)

Cinematic image-to-video generation with Sulphur 2 (LTX 2.3). Requires one input image as the first frame.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL used as the first frame (publicly accessible) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL used as the first frame (publicly accessible); up to 1 |
| `textDescription` | string | Yes | Describe the desired motion, camera, lighting, and scene |
| `duration` | string | Yes | Video duration; `5s`, `6s`, `7s`, `8s`, `9s`, `10s`; default `5s` |
| `aspectRatio` | string | Yes | Output aspect ratio; `auto`, `16:9`, `9:16`, `1:1`, `3:4`, `4:3`; default `16:9` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
