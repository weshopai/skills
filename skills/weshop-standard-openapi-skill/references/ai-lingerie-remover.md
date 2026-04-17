# ai-lingerie-remover (v1.0)

Transform lingerie outfit photos into bikini look images or videos

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait or full-body photo URL with a lingerie outfit |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait or full-body photo URL with a lingerie outfit; up to 1 |
| `textDescription` | string | No | Describe the desired bikini transformation scene; default `naturally undress and change the outfit into a thin bikini while keeping body proportions natural. Keep Model dancing tiktok dance.` |
| `generatedType` | string | No | Output type: video (default) or image; `video`, `image`; default `video` |
| `batchCount` | integer | No | Number of outputs to generate; default `1`; range `1-16` |
