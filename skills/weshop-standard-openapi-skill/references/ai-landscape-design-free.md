# ai-landscape-design-free (v1.0)

Redesign a yard or outdoor space with a new landscape style

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Image URLs: image 1 = yard to redesign, image 2 = style reference (both optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Image URLs: image 1 = yard to redesign, image 2 = style reference (both optional); up to 2 |
| `textDescription` | string | No | Describe the desired landscape style; default `You are a professional landscape designer. Your task is to create a new [Modern style] landscape design for this yard. You need to retain the materials and core structure of the yard while upgrading the landscape to make it modern, beautiful, and practical.  *If image2 exists, you should integrate the style of image2.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
