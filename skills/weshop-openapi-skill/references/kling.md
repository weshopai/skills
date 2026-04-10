# kling (v1.0)

AI video generation from images and text using Kling

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Reference image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Reference image URL; up to 1 |
| `textDescription` | string | Yes | Describe the desired motion or scene |
| `modelName` | string | No | Kling model version; `Kling_3_0`, `Kling_2_6`, `Kling_2_5_Turbo`, `Kling_2_1_Master`, `Kling_2_1`; default `Kling_3_0` |
| `duration` | string | No | Video duration (Kling_3_0: 3s-15s; others: 5s, 10s); default `5s` |
| `generateAudio` | string | No | Generate audio (Kling_3_0 and Kling_2_6 only); `true`, `false` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
