# virtualtryon (v1.0)

Virtual try-on composition with optional model/location references

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Garment image URL |
| `input.fashionModelImage` | string(url) | No | Model reference image URL — the generated model will resemble this person |
| `input.locationImage` | string(url) | No | Background reference image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `originalImage` | string | Yes | Garment image URL |
| `fashionModelImage` | string | No | Model reference image URL — the generated model will resemble this person |
| `locationImage` | string | No | Background reference image URL |
| `generateVersion` | string | Yes | Generation engine. weshopFlash: fast; weshopPro: high quality, supports aspectRatio; bananaPro: requires imageSize, supports aspectRatio; `weshopFlash`, `weshopPro`, `bananaPro` |
| `descriptionType` | string | Yes | Prompt mode. auto: system generates prompt automatically; custom: you provide textDescription (required); `auto`, `custom` |
| `textDescription` | string | No | Text description of desired result. Required when descriptionType=custom. Use 'Figure 1' for originalImage, 'Figure 2' for fashionModelImage, 'Figure 3' for locationImage |
| `aspectRatio` | string | No | Output aspect ratio. Valid for weshopPro and bananaPro only; `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `9:16`, `16:9`, `21:9` |
| `imageSize` | string | No | Output resolution. Required when generateVersion=bananaPro; `1K`, `2K`, `4K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
