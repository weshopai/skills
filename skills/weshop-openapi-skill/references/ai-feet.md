# ai-feet (v1.0)

Generate a realistic low-angle bare feet photo from a portrait

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait or full-body image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait or full-body image URL; up to 1 |
| `textDescription` | string | No | Custom feet scene instruction; default `Low angle view of the subject's bare feet with no shoes, while subject sits in an chair. Foreground focus on the soles, background focus on the subject, keep original body proportion and reasonable posture.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
