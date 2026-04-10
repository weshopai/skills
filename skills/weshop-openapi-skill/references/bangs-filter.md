# bangs-filter (v1.0)

Add natural-looking bangs to a person's hairstyle

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom bangs style instruction; default `Give this person bangs naturally, don't change their hair color.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
