# pregnant_ai (v1.0)

Visualize how a person would look pregnant

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Input portrait image URL |
| `textDescription` | string | No | Custom pregnancy transformation instruction; default `Imagine what this person would look like when she is pregnant for 8 months. Don't change her outfit or her appearance.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
