# kling (v1.0)

AI video generation from images and text using Kling. Pass one image for first-frame image-to-video, or two images for first frame + last frame.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | First-frame image URL, plus optional last-frame image URL (image 1 = first frame, image 2 = last frame) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | First-frame image URL, plus optional last-frame image URL (image 1 = first frame, image 2 = last frame). Last frame is supported for Kling_3_0, Kling_2_6, Kling_2_5_Turbo, and Kling_2_1; up to 2 |
| `textDescription` | string | Yes | Describe the desired motion or scene |
| `modelName` | string | No | Kling model version; `Kling_3_0`, `Kling_2_6`, `Kling_2_5_Turbo`, `Kling_2_1_Master`, `Kling_2_1`; default `Kling_3_0` |
| `duration` | string | No | Video duration (Kling_3_0: 3s-15s; others: 5s, 10s); default `5s` |
| `generateAudio` | string | No | Generate audio (Kling_3_0 and Kling_2_6 only); `true`, `false` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
