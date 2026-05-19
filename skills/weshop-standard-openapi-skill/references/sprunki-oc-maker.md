# sprunki-oc-maker (v1.0)

Create a Sprunki-style original character from a person photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Custom Sprunki OC description; default `Transform the person in the uploaded photo into a Sprunki-style original character (OC). Keep the same facial identity, hairstyle, and key proportions, while redesigning the character in a colorful, playful Sprunki cartoon aesthetic. Big expressive eyes, simplified geometric shapes, smooth outlines, vibrant pastel color palette, soft shading, clean vector-like rendering, cute and energetic mood, stylized costume details, character sheet illustration quality, centered composition, high detail, 4k, masterpiece.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
