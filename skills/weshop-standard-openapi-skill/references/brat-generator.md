# brat-generator (v1.0)

Create a brat-style album cover meme with custom text and color

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URL (optional); up to 1 |
| `textDescription` | string | No | Describe the brat cover; default `a pure [color] background with text [Brat] on it. 1:1 ratio.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
