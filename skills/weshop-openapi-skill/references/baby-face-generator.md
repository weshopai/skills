# baby-face-generator (v1.0)

Predict what a baby would look like from two parent photos

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Parent photo URLs (up to 2, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Parent photo URLs (up to 2, optional); up to 2 |
| `textDescription` | string | No | Custom baby generation instruction; default `Generate a realistic photo of a [female] baby based on the two uploaded parent photos. Blend the facial features, skin tones, ethnic characteristics and any specific feature from both parents to create a natural-looking child. Child photo only.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
