# ai-headshot-generator (v1.0)

Create professional ID-style or business headshots from a single portrait image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL (publicly accessible) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL (publicly accessible); up to 1 |
| `textDescription` | string | Yes | Custom headshot style and composition instructions; default `Crop the head and create a 2-inch ID photo in [offical Travel ID style] with: [white background];[Professional business attire], maintain exact facial features` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
