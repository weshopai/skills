# ai-tattoo-generator (v1.0)

Create a tattoo design try-on from text or reference image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired tattoo design and placement; default `Generate aline art style single piece no color tattoo design try-on, small, on arm.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
