# ai-christmas-photo (v1.0)

Transform a portrait into a festive Christmas scene

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input portrait image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input portrait image URL; up to 1 |
| `textDescription` | string | No | Custom Christmas scene instruction; default `Create a Christmas-themed portrait photo based on the provided image. The overall scene should convey a festive Christmas party atmosphere, incorporating classic Christmas decorative elements such as gift boxes, bells, apples, and snowmen. Must include a decorated Christmas tree with hanging ornaments, a small teddy bear plush placed nearby, and a large Santa Claus plush toy positioned in the background. In the foreground, golden confetti and falling snow should be visible, featuring motion blur effects to enhance the sense of movement and festivity. The photography style should use direct on-camera flash, creating a bold, frontal lighting effect. The overall aesthetic should evoke a vintage film look with subtle Y2K influences, featuring visible film grain and noise texture. Emphasize catchlights in the eyes as much as possible. The primary color palette should consist of vivid red, green, and white, with optional dark blue accents. The background vary between a white wall, a photo studio, a deep night sky filled with stars, or others as long as it aligns with a Christmas theme. The shot type can be randomly chosen between medium shot, full-body shot, or close-up. For wardrobe styling, select Christmas-themed outfits, such as Christmas sweaters, Santa hats, red scarves, or winter attire. The original facial details and body proportions of the subject must be strictly preserved.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
