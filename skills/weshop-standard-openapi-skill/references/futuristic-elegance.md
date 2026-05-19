# futuristic-elegance (v1.0)

Cinematic sci-fi outfit transformation with futuristic harajuku fashion

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom style instruction; default `Put this person in a dramatic cinematic scene with harajuku fashion with futuristic color PVC clothing, semi-transparent color vinyl, metalic prismatic, holographic, chromatic aberration, fashion illustration, masterpiece. slightly wide-angle lens, natural soft key lighting, realistic style. Make it look like an actual movie scene, but keep original aspect ratio.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
