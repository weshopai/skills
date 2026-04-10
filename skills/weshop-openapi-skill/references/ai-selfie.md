# ai-selfie (v1.0)

Transform a portrait into a natural iPhone-style selfie photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom selfie scene instruction; default `Generate a selfie shot, wide angle, iphone style, no need to show the phone.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
