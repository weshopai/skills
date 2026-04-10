# ai-3d-rendering (v1.0)

Transform a photo into a Blender-style 3D model viewport screenshot

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input image URL; up to 1 |
| `textDescription` | string | No | Custom 3D rendering instruction; default `A screenshot of a 3D modeling software interface, showing the Blender viewport. At the center of the scene is a highly realistic 3D model of the main subject of this image in full and realistic rendering, with no visible topology or wireframe. The model is placed on a gray 3D grid ground with an infinite horizon. The software UI toolbars are visible along the side, a coordinate axis widget appears in the corner, the viewport is in solid shading mode, and the overall scene represents a 3D asset design workspace. 4k resolution and ratio.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
