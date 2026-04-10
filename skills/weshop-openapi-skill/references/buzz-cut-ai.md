# buzz-cut-ai (v1.0)

Change a person's hairstyle to a buzz cut

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom hairstyle instruction; default `Change the hairstyle to a buzz cut.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
