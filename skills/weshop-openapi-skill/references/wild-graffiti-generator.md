# wild-graffiti-generator (v1.0)

Create wild-style spray paint graffiti art from text or image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | No | Reference image URL (optional) |
| `textDescription` | string | No | Describe the desired graffiti style or text; default `wild style graffiti, spray paint texture, artistic chaos, plain background.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
