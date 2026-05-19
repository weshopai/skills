# ai-couple-photo-maker (v1.0)

Create a realistic romantic couple photo by combining two portrait images into a single scene

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Two portrait image URLs (publicly accessible) to combine into a romantic couple photo |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Two portrait image URLs (publicly accessible) to combine into a romantic couple photo; up to 2 |
| `textDescription` | string | No | Custom instructions for how the couple photo should look; default `Combine the two uploaded portraits into one romantic couple's photo, sitting close together, natural lighting, realistic style` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
