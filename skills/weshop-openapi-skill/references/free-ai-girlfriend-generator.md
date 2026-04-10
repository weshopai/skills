# free-ai-girlfriend-generator (v1.0)

Generate a realistic AI girlfriend portrait from text or reference image

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired girlfriend portrait; default `A random AI girlfriend portrait, beautiful young woman, {ethnicity}, {hairstyle}, {makeup}, {vibe}, gentle soft smile, natural skin texture, cinematic soft lighting, {scene}, shallow depth of field, realistic photography, emotional warm atmosphere, 50mm lens, f1.8, ultra-detailed, 4k, masterpiece.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
