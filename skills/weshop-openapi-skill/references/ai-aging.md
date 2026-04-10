# ai-aging (v1.0)

AI age progression on portrait photos

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom aging instruction; default `what will this person look like when he/she is 60` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
