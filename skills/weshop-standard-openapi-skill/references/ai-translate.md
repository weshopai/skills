# ai-translate (v1.0)

Translate text in an image to another language while preserving design

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image containing text URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image containing text URL; up to 1 |
| `textDescription` | string | No | Custom translation instruction; default `Translate all text in this image to English. Keep the same design and aesthetics to maintain the style of the image. Don't simply put the text on the new image, try to generate text as original.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
