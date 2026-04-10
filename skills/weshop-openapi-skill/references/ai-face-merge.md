# ai-face-merge (v1.0)

Blend two faces together into a single realistic portrait

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Two face image URLs: image 1 and image 2 (baseline) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Two face image URLs: image 1 and image 2 (baseline); up to 2 |
| `textDescription` | string | No | Custom merge instruction (reference images as 'image 1' and 'image 2'); default `Analyze the characteristics of these two faces, try imagine the person with both face features merged together. Don't simply put the face on the other image, try to generate a merged face. Keep Image 2 as the baseline.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
