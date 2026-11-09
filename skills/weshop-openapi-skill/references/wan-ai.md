# wan-ai (v1.0)

Wan video generation. Omit modelName to preserve Wan 2.5: one image, 5s. Explicit Wan_3_0_Reference supports text or up to 10 images, 5 videos, 5 audios (20 total), including audio-only references. Wan_3_0_I2V requires 1-2 first/last images and no video/audio references. Wan 3.0 defaults: 5s, 720P, adaptive, generateAudio true; duration 2s-30s.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Public image URLs. Wan 2.5 requires exactly one; 3.0 Reference supports up to 10 optional references; 3.0 I2V requires 1-2 ordered first/last frames. |
| `input.videos` | array | No | Public reference video URLs, Wan 3.0 Reference only. Each clip 1-15s, video total <=15s, input video + output <=30s. Local video upload is unsupported. |
| `input.audios` | array | No | Public reference audio URLs, Wan 3.0 Reference only. Each clip 1-15s, audio total <=15s. Local audio upload is unsupported. |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Public image URLs. Wan 2.5 requires exactly one; 3.0 Reference supports up to 10 optional references; 3.0 I2V requires 1-2 ordered first/last frames.; up to 10 |
| `textDescription` | string | Yes | Describe the desired video scene |
| `duration` | string | No | Video duration. Wan 2.5: 3s-8s; Wan 3.0: 2s-30s.; default `5s` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
| `modelName` | string | No | Optional model; omission keeps historical Wan 2.5 behavior.; `Wan_2_5`, `Wan_3_0_Reference`, `Wan_3_0_I2V`; default `Wan_2_5` |
| `videos` | array | No | Public reference video URLs, Wan 3.0 Reference only. Each clip 1-15s, video total <=15s, input video + output <=30s. Local video upload is unsupported.; up to 5 |
| `audios` | array | No | Public reference audio URLs, Wan 3.0 Reference only. Each clip 1-15s, audio total <=15s. Local audio upload is unsupported.; up to 5 |
| `resolution` | string | No | Wan 3.0 only, defaults to 720P; CLI also accepts lowercase p.; `480P`, `720P`, `1080P` |
| `aspectRatio` | string | No | Wan 3.0 only, defaults to adaptive; I2V requires adaptive.; `adaptive`, `16:9`, `4:3`, `1:1`, `3:4`, `9:16` |
| `generateAudio` | string | No | Wan 3.0 only, defaults to true.; `true`, `false` |
