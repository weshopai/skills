# ghibli-art-create (v1.0)

Transform photos into Studio Ghibli anime art style

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Input image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Input image URL (optional); up to 1 |
| `textDescription` | string | No | Custom Ghibli style instruction; default `Turn this image into ghibli style` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
