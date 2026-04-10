# gender-swap (v1.0)

Transform a portrait to the opposite gender while preserving identity

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom gender transformation instruction; default `Change this person's gender to the opposite one.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
