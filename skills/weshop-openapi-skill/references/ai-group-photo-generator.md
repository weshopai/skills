# ai-group-photo-generator (v1.0)

Create a creative group photo or collage from up to 10 images

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Reference image URLs (up to 10) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Reference image URLs (up to 10); up to 10 |
| `textDescription` | string | No | Custom group photo or collage style instruction; default `Please don't change any elements that I provide. Generate a chaotic and creative multi-media collage with a completely randomized aesthetic. Combine a wide array of contrasting elements: vintage magazine cutouts, neon-colored glitch art, 19th-century botanical illustrations, and sharp vector geometric shapes. The composition should be an experimental mix of textures—including torn glossy paper, rough cardboard, transparent celluloid film, and metallic foil. Incorporate a clashing color palette that shifts randomly across the canvas. Features an unpredictable focal point, layered with 3D drop shadows to create a sense of physical depth. High resolution, maximalist detail, eclectic and avant-garde style.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
