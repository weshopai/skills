# ai-clothes-changer (v1.0)

Dress a person in the garment shown in another photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Two image URLs: image 1 = person, image 2 = garment/outfit |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Two image URLs: image 1 = person, image 2 = garment/outfit; up to 2 |
| `textDescription` | string | No | Custom clothing instruction (reference images as 'image 1' and 'image 2'); default `The person in Figure 1 is wearing the clothes shown in Figure 2` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
