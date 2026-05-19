# ai-blemish-remover (v1.0)

Remove facial blemishes such as acne and spots while preserving natural skin texture and lighting

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL (publicly accessible) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL (publicly accessible); up to 1 |
| `textDescription` | string | Yes | Custom blemish removal instructions; default `remove facial imperfections and acne spots, keep natural skin texture and facial expression, preserve identity and lighting` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
