# ai-spray-paint (v1.0)

Convert a photo into a black-and-white spray paint stencil

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Input image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Input image URL (optional); up to 1 |
| `textDescription` | string | No | Custom stencil instruction; default `Change the original photo to stencil style, only black and white, spray paint style.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
