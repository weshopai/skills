# fat-ai (v1.0)

Visualize how a person would look extremely overweight

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom body transformation instruction; default `Give me a look of how this person would look when this person became extremely fat. Don't change clothes and appearance.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
