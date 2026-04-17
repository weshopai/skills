# ai-poster-from-images (v1.0)

Create a designed poster from up to 5 reference images

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URLs (up to 5, optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URLs (up to 5, optional); up to 5 |
| `textDescription` | string | No | Describe the desired poster; default `Make a poster based on the uploaded picture and user instructions. Based on the uploaded image, determine the main color of the brand. If not available, you can use the main color of the product. The poster design should conform to the aesthetic standards of modern design styles, try to be simple and elegant. Font should have difference in sizes and a fitting style for good aesthetics.` |
| `aspectRatio` | string | No | Output aspect ratio; `1:1`, `2:3`, `3:2`, `4:3`, `3:4`, `16:9`, `9:16`, `21:9`; default `1:1` |
| `imageSize` | string | No | Output resolution; `1K`, `2K`, `4K`; default `1K` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
