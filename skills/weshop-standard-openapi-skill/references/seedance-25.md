# seedance-25 (v1.0)

Seedance 2.5 native 4–30s cinematic video generation from text, with optional reference images, videos, and audio

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Optional reference image URLs (publicly accessible, up to 30). Refer to them in the prompt as image 1, image 2, etc. |
| `input.videos` | array | No | Optional reference video URLs (publicly accessible, up to 10) |
| `input.audios` | array | No | Optional reference audio URLs (publicly accessible, up to 10) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Optional reference image URLs (publicly accessible, up to 30). Refer to them in the prompt as image 1, image 2, etc.; up to 30 |
| `videos` | array | No | Optional reference video URLs (publicly accessible, up to 10); up to 10 |
| `audios` | array | No | Optional reference audio URLs (publicly accessible, up to 10); up to 10 |
| `textDescription` | string | Yes | Describe the desired video scene, motion, camera, and audio |
| `modelName` | string | Yes | Seedance 2.5 model; `Seedance_25`; default `Seedance_25` |
| `duration` | string | Yes | Video duration (native single-segment, 4s-30s); `4s`, `5s`, `6s`, `7s`, `8s`, `9s`, `10s`, `11s`, `12s`, `13s`, `14s`, `15s`, `16s`, `17s`, `18s`, `19s`, `20s`, `21s`, `22s`, `23s`, `24s`, `25s`, `26s`, `27s`, `28s`, `29s`, `30s`; default `4s` |
| `aspectRatio` | string | Yes | Output aspect ratio; `21:9`, `16:9`, `9:16`, `3:4`, `4:3`, `1:1`; default `3:4` |
| `generateAudio` | string | Yes | Generate native audio; `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
