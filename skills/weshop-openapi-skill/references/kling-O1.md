# kling-O1 (v1.0)

Kling O1 cinematic video generation with Reference mode (text + multimodal references) or Image-to-Video (first/last frame)

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference or frame image URLs (publicly accessible, optional). Kling_Video_O1_Ele: up to 4 references. Kling_Video_O1_I2V: image 1 = first frame, image 2 = last frame. |
| `input.videos` | array | No | Optional reference video URL (publicly accessible; mainly for Kling_Video_O1_Ele) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference or frame image URLs (publicly accessible, optional). Kling_Video_O1_Ele: up to 4 references. Kling_Video_O1_I2V: image 1 = first frame, image 2 = last frame.; up to 4 |
| `videos` | array | No | Optional reference video URL (publicly accessible; mainly for Kling_Video_O1_Ele); up to 1 |
| `textDescription` | string | Yes | Describe the desired video, motion, or edit |
| `modelName` | string | Yes | Kling O1 mode: Reference (text + multimodal references) or Image to Video (first/last frame); `Kling_Video_O1_Ele`, `Kling_Video_O1_I2V`; default `Kling_Video_O1_Ele` |
| `duration` | string | Yes | Video duration; `3s`, `4s`, `5s`, `6s`, `7s`, `8s`, `9s`, `10s`; default `5s` |
| `aspectRatio` | string | Yes | Output aspect ratio (used by Kling_Video_O1_Ele; hidden when a reference video is provided); `9:16`, `16:9`, `1:1`; default `9:16` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
