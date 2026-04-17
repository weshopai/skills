# clothing-magic-remover (v1.0)

Erase accessories or partial clothing while keeping textures realistic

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input person photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input person photo URL; up to 1 |
| `textDescription` | string | No | Describe what clothing to remove; default `undress the outfit into sexy bikini while keeping body proportions natural.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
