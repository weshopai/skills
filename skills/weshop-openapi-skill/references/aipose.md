# aipose (v1.0)

Keep the garment but change the human pose

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Source image URL |
| `textDescription` | string | Yes | Pose instruction describing the desired pose |
| `generateVersion` | string | No | Generation quality. lite: fast (default); pro: higher quality, slower; `lite`, `pro`; default `lite` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
