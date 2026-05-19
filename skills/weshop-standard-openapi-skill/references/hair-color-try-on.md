# hair-color-try-on (v1.0)

Change a person's hair color while preserving hairstyle and details

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom hair color instruction; default `Change hair color naturally. choose whatever suit the person's skin tone or randomly between Rose Gold/Pinkish Brown/Dark Blue. Don't change hair style or other details.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
