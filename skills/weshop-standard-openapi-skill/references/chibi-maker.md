# chibi-maker (v1.0)

Convert a photo into a cute chibi character sticker

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input photo URL; up to 1 |
| `textDescription` | string | No | Custom chibi style instruction; default `Turn this photo into a chibi sticker.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
