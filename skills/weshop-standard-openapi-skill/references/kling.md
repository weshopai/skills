# kling (v1.0)

Kling video generation. CLI/OpenAPI omission preserves Kling_3_0, 5s, first/last-frame semantics; Web omission selects Kling_4_0_Reference, 10s, 1080p. Select 4.0 explicitly via modelName. Reference accepts text/image/video references; I2V accepts text or first/last/middle keyframes. 4.0 has no audio references or generateAudio option.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Public image URLs. Legacy: required 1-2 first/last frames (Master only one). 4.0 Reference: optional, up to 10 references. 4.0 I2V: optional first and last frame, at most 2; use middleFrames for intermediate frames. |
| `input.videos` | array | No | Public reference video URLs, only Kling_4_0_Reference. Local video upload is unsupported. |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Public image URLs. Legacy: required 1-2 first/last frames (Master only one). 4.0 Reference: optional, up to 10 references. 4.0 I2V: optional first and last frame, at most 2; use middleFrames for intermediate frames.; up to 10 |
| `textDescription` | string | Yes | Describe the desired motion or scene |
| `modelName` | string | No | CLI/OpenAPI default remains Kling_3_0; Web default is Kling_4_0_Reference. Explicit model selection wins.; `Kling_3_0`, `Kling_2_6`, `Kling_2_5_Turbo`, `Kling_2_1_Master`, `Kling_2_1`, `Kling_4_0_Reference`, `Kling_4_0_I2V`; default `Kling_3_0` |
| `duration` | string | No | Legacy CLI default 5s (3.0: 3s-15s; others: 5s/10s); Kling 4.0 default 10s, supports 3s-30s. Omit to use the selected model default. |
| `generateAudio` | string | No | Legacy Kling_3_0 and Kling_2_6 audio only; do not send for Kling 4.0.; `true`, `false` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
| `videos` | array | No | Public reference video URLs, only Kling_4_0_Reference. Local video upload is unsupported.; up to 5 |
| `firstFrame` | string | No | Public first-frame image URL, only Kling_4_0_I2V; do not combine with images. |
| `lastFrame` | string | No | Public last-frame image URL, only Kling_4_0_I2V; do not combine with images. |
| `middleFrames` | array | No | Kling_4_0_I2V intermediate frames in order, with public image URLs and optional unique IDs. CLI --middle-frames takes a JSON array; up to 10 total keyframe images including first/last.; up to 10 |
| `resolution` | string | No | Kling 4.0 only; defaults to 1080p when omitted.; `720p`, `1080p` |
| `aspectRatio` | string | No | Kling 4.0 only. Omit for endpoint default: text 16:9, Reference with media adaptive, I2V frames determine ratio. With keyframes only omitted/empty/adaptive is allowed.; ``, `adaptive`, `21:9`, `16:9`, `9:16`, `1:1` |
