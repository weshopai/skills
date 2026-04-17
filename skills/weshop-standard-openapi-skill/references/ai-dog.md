# ai-dog (v1.0)

Create or transform pet photos with AI

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Input pet photo URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Input pet photo URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired pet scene or transformation; default `Pet taking a bath. Maintain realistic proportions including the number of limbs.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
