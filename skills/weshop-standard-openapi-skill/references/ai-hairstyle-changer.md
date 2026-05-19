# ai-hairstyle-changer (v1.0)

Change a person's hairstyle from a photo or text description

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired hairstyle; default `Change to ［short hair］` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
