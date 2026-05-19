# ai-flag-generator (v1.0)

Create a custom flag design from text or a reference image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image for the flag design URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image for the flag design URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired flag design; default `A random flag design with metallic insignia, realistic fabric folds, and suitable background.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
