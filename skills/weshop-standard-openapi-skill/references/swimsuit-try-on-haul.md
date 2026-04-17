# swimsuit-try-on-haul (v1.0)

Transform a person photo into a swimsuit try-on image or video

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait or full-body photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait or full-body photo URL; up to 1 |
| `textDescription` | string | No | Describe the desired swimsuit scene; default `naturally undress and change the outfit into a thin bikini while keeping body proportions natural. Keep Model dancing tiktok dance.` |
| `generatedType` | string | No | Output type: video (default) or image; `video`, `image`; default `video` |
| `batchCount` | integer | No | Number of outputs to generate; default `1`; range `1-16` |
