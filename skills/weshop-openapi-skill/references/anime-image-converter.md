# anime-image-converter (v1.0)

Transform any photo into anime art style

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | No | Custom anime style instruction; default `Turn this photo into anime.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
