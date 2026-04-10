# mugshot-creator (v1.0)

Generate a police-style mugshot photo from a portrait

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom mugshot instruction; default `Generate a mugshot of this person, height measurement background, keep face and appearance detail.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
