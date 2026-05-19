# midjourney (v1.0)

Image generation using Midjourney v6.1, v7, or Niji 6

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URL (optional); up to 1 |
| `textDescription` | string | Yes | Describe the desired image |
| `modelName` | string | No | Midjourney model version; `Midjourney_6_1`, `Midjourney_7`, `Midjourney_Niji_6`; default `Midjourney_6_1` |
| `aspectRatio` | string | No | Output aspect ratio; `1:1`, `4:3`, `3:4`, `16:9`, `9:16`; default `1:1` |
