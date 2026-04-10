# celeb-ai (v1.0)

Place a person in a selfie with a celebrity or fictional character

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URLs (up to 2) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URLs (up to 2); up to 2 |
| `textDescription` | string | No | Describe the celebrity or character and scene; default `Take a selfie angle photo of this person and Harry Potter. No need to show the phone. choose appropriate background.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
