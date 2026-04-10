# ai-image-combiner (v1.0)

Naturally merge two photos into a single cohesive image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Two image URLs to combine (image 1 and image 2) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Two image URLs to combine (image 1 and image 2); up to 2 |
| `textDescription` | string | No | Custom merge instruction (reference images as 'image 1' and 'image 2'); default `Merge these two photos together naturally. Don't simply put element on the another image, try to generate a merged photo.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
