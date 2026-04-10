# square-face-icon-generator (v1.0)

Create a minimalist anime-style square face avatar from a photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference portrait image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference portrait image URL (optional); up to 1 |
| `textDescription` | string | No | Custom face icon description; default `A minimalist flat-art vector illustration of a stylized anime face, Japanense style drawing. The face must be a square close-up 1:1 ratio, no background. No gradients, solid colors only, 2D minimalist aesthetic, no background.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
