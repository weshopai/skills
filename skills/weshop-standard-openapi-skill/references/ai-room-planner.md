# ai-room-planner (v1.0)

Redesign a room photo with a new interior design style

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Input room photo URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Input room photo URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired interior design style; default `Identify the room type, layout, key furniture objects, clutter, and windows from the source. Redesign the room  in [modern style] without changing major decoration. Keep room structure and window position. Implement a clean, integrated modern palette.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
