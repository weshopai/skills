# demon-slayer-oc-maker (v1.0)

Transform a person into a Kimetsu no Yaiba anime character

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Custom Demon Slayer OC description; default `Turn this person into Demon Slayer anime style, Kimetsu no Yaiba aesthetics, thick brush strokes, bold black outlines, expressive eyes with distinct pupils, wearing a custom slayer uniform and a patterned haori, Ufotable high-quality animation style, cinematic lighting, sharp focus, vibrant cel-shading, keep key facial and gender characteristics.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
