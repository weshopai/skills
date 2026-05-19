# 2d-to-3d-image-converter (v1.0)

Transform a 2D image into a 3D rendered version

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input 2D image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input 2D image URL; up to 1 |
| `textDescription` | string | No | Custom 3D conversion instruction; default `Convert the uploaded 2d image into a 3d image based on the user instructions.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
