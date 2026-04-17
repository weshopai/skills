# outfit-generator (v1.0)

Redesign a complete outfit on a person photo based on style prompt

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input person photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input person photo URL; up to 1 |
| `textDescription` | string | No | Describe the desired outfit style; default `Design an complete new and recommended outfit based on the uploaded photo. Keep original face and body proportion, keep original pose and background; Keep original image composition; select the proper texture used for outfit. No annotations required.
1. Analyze the core characteristics of the model, dressing style and potential personality of the subject.
2. Extract the disassemblable first-level elements (coat, shoes, big expression)
3. Generate a composite diagram containing all these elements, ensuring accurate perspective, unified lighting and shadow, keep everything else same.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
