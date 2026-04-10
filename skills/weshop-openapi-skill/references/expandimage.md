# expandimage (v1.0)

Expand the canvas to a target size. The original image is placed within the new canvas and the added area is filled by AI generation, not stretching.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Source image URL |
| `targetWidth` | integer | Yes | Target canvas width in pixels; max 4096; max `4096` |
| `targetHeight` | integer | Yes | Target canvas height in pixels; max 4096; max `4096` |
| `fillLeft` | integer | No | Horizontal offset (px) from left edge of canvas to left edge of original image. Defaults to centered |
| `fillTop` | integer | No | Vertical offset (px) from top edge of canvas to top edge of original image. Defaults to centered |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
