# image-to-sketch (v1.0)

Convert a photo into a rough pencil sketch

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | No | Custom sketch style instruction; default `Turn this image into rough pencil sketch without changing details.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
