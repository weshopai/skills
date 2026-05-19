# bald-filter (v1.0)

Make a person appear bald while preserving facial details

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom instruction; default `Change the hairstyle to bald. Don't change any other detail or face.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
