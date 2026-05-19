# braces-filter (v1.0)

Add dental braces to a person's teeth in a portrait photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom braces instruction; default `Add braces in this person's tooth` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
