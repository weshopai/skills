# ps2-filter (v1.0)

Transform a photo into a retro PS2-era Sims game character

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom PS2 game style instruction; default `Turn this person into a PS2 Sims game character. 3D but blurry texture, try replicate exactly as the game.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
