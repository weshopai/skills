# minimax-h3 (v1.0)

MiniMax H3 multimodal video generation in Reference mode (images/videos/audios) or Image-to-Video (first/last frame). I2V requires 1–2 images and adaptive aspect ratio.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference or frame image URLs (publicly accessible). MiniMax_H3_I2V: 1–2 images (image 1 = first frame, image 2 = last frame). MiniMax_H3_Reference: up to 9 optional references. |
| `input.videos` | array | No | Optional reference video URLs (publicly accessible, up to 3). Supported in Reference mode only; not allowed for MiniMax_H3_I2V. |
| `input.audios` | array | No | Optional reference audio URLs (publicly accessible, up to 3). Supported in Reference mode only; not allowed for MiniMax_H3_I2V. |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference or frame image URLs (publicly accessible). MiniMax_H3_I2V: 1–2 images (image 1 = first frame, image 2 = last frame). MiniMax_H3_Reference: up to 9 optional references.; up to 9 |
| `videos` | array | No | Optional reference video URLs (publicly accessible, up to 3). Supported in Reference mode only; not allowed for MiniMax_H3_I2V.; up to 3 |
| `audios` | array | No | Optional reference audio URLs (publicly accessible, up to 3). Supported in Reference mode only; not allowed for MiniMax_H3_I2V.; up to 3 |
| `textDescription` | string | Yes | Describe the desired video, motion, camera, and audio |
| `modelName` | string | Yes | MiniMax H3 mode; `MiniMax_H3_Reference`, `MiniMax_H3_I2V`; default `MiniMax_H3_Reference` |
| `duration` | string | Yes | Video duration; `5s`, `6s`, `7s`, `8s`, `9s`, `10s`, `11s`, `12s`, `13s`, `14s`, `15s`; default `5s` |
| `aspectRatio` | string | Yes | Output aspect ratio. I2V models must use adaptive. In Reference mode, adaptive is locked when a video is present; if there is no image/video input, adaptive falls back to 16:9.; `adaptive`, `21:9`, `16:9`, `4:3`, `1:1`, `3:4`, `9:16`; default `adaptive` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
