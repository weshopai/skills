# ai-elf (v1.0)

Transform a portrait into a fantasy elf character

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom elf transformation instruction; default `Turn this person into an elf` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
