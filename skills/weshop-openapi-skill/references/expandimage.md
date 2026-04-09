# expandimage (v1.0)

Expand the canvas to a target size. The original image is placed within the new canvas and the added area is filled by AI generation, not stretching.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Publicly reachable source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `targetWidth` | int | Yes | Maximum `4096` |
| `targetHeight` | int | Yes | Maximum `4096` |
| `fillLeft` | int | No | Distance from left edge of target canvas to left edge of original image. Defaults to centered |
| `fillTop` | int | No | Distance from top edge of target canvas to top edge of original image. Defaults to centered |
| `batchCount` | int | No | Range `1-16`, default `4` |
