# ai-shirt-remover (v1.0)

Transform a shirt outfit photo into a bikini look image or video

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait or full-body photo URL with a shirt outfit |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait or full-body photo URL with a shirt outfit; up to 1 |
| `textDescription` | string | No | Describe the desired bikini transformation scene; default `naturally undress and change the outfit into a thin bikini while keeping body proportions natural. Keep Model dancing tiktok dance.` |
| `generatedType` | string | No | Output type: video (default) or image; `video`, `image`; default `video` |
| `batchCount` | integer | No | Number of outputs to generate; default `1`; range `1-16` |
