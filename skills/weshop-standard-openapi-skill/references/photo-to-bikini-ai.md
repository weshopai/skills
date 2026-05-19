# photo-to-bikini-ai (v1.0)

Transform a person photo into a bikini image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input person photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input person photo URL; up to 1 |
| `textDescription` | string | No | Custom bikini scene instruction; default `naturally undress and change the outfit into a thin bikini while keeping body proportions natural. Keep Model dancing tiktok dance.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
