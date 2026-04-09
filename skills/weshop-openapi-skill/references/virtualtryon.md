# virtualtryon (v1.0)

Virtual try-on composition with optional model/location references.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | The garment to preserve in the result |
| `input.fashionModelImage` | string(url) | No | Model reference image; generated model will resemble this person |
| `input.locationImage` | string(url) | No | Background reference image |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `generateVersion` | string | Yes | `weshopFlash`, `weshopPro`, or `bananaPro` |
| `descriptionType` | string | Yes | `custom` or `auto` |
| `textDescription` | string | Conditional | Required when `descriptionType=custom`. Use `Figure 1` for `originalImage`, `Figure 2` for `fashionModelImage`, `Figure 3` for `locationImage` |
| `aspectRatio` | string | Conditional | Valid for `weshopPro` and `bananaPro`: `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `9:16`, `16:9`, `21:9` |
| `imageSize` | string | Conditional | Required when `generateVersion=bananaPro`: `1K`, `2K`, `4K` |
| `batchCount` | int | No | Range `1-16`, default `4` |
