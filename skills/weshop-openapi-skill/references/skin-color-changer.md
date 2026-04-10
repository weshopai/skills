# skin-color-changer (v1.0)

Change a person's skin tone while preserving face details

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom skin tone instruction; default `Change skin tone to a healthy wheat color while keeping original face detail and lighting composition.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
