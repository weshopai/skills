# murder-drones-oc (v1.0)

Transform a person into a Murder Drones-inspired robotic drone character

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Custom Murder Drones OC description; default `Convert the person from the reference image into a Murder Drones inspired OC. Strictly maintain facial identity, head shape, and signature traits, while transforming the body into an elegant yet dangerous robotic drone form. Smooth black metal armor, luminous LED accents, claw-like fingers, floating mechanical components, glowing visor or eyes, dark cyberpunk environment, cinematic lighting, high detail sci-fi illustration, clean composition, 4k, character concept art, masterpiece.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
