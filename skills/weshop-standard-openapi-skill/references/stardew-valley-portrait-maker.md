# stardew-valley-portrait-maker (v1.0)

Create a Stardew Valley game-style character portrait

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference portrait image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference portrait image URL (optional); up to 1 |
| `textDescription` | string | No | Custom character description; default `Generate a Stardew Valley Style Head Portrait image, 1:1 ratio, 45 angle toward left, try to replicate exactly as the game.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
