# photo-wrinkle-remover (v1.0)

Smooth facial wrinkles in portrait photos while preserving natural skin texture and facial identity

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL (publicly accessible) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL (publicly accessible); up to 1 |
| `textDescription` | string | Yes | Custom wrinkle removal instructions (what to smooth and what to preserve); default `Remove wrinkles from this person` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
