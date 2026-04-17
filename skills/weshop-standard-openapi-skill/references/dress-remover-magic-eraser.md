# dress-remover-magic-eraser (v1.0)

Erase a dress and replace with a bikini while keeping body proportions

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input person photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input person photo URL; up to 1 |
| `textDescription` | string | No | Describe what to remove and replace; default `undress the outfit into sexy bikini while keeping body proportions natural.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
