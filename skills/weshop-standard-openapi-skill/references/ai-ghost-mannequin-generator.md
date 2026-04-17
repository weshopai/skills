# ai-ghost-mannequin-generator (v1.0)

Create a professional ghost mannequin effect from a clothing photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input clothing photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input clothing photo URL; up to 1 |
| `textDescription` | string | No | Custom ghost mannequin instruction; default `Transform the clothing from the image into a professional "ghost mannequin" photography effect. Remove the original model or body completely. The garment should appear hollow and three-dimensional, retaining the shape as if worn by an invisible form. Clearly show the inside of the neck opening, cuffs, and hem, revealing the inner fabric texture and labels. The clothing is floating against a clean, pure white studio background. Soft studio lighting emphasizes fabric folds and texture.` |
| `aspectRatio` | string | No | Output aspect ratio; `auto`, `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `1:1` |
| `imageSize` | string | No | Output resolution; `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
