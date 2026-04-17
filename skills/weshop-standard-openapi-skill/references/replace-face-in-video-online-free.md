# replace-face-in-video-online-free (v1.0)

Replace a face in a video with a reference face photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.videos` | array | Yes | Input video URL |
| `input.images` | array | Yes | Reference face photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Reference face photo URL; up to 1 |
| `videos` | array | Yes | Input video URL; up to 1 |
| `batchCount` | integer | No | Number of outputs to generate; default `1`; range `1-16` |
