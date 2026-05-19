# ai-action-figure-generators (v1.0)

Turn a photo or character into a collectible action figure display

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference character or person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference character or person image URL (optional); up to 1 |
| `textDescription` | string | No | Custom action figure description; default `A commercially available figure of the character from the illustration is produced in 1/ scale, featuring a realistic style and environment. The figure is displayed on a computer desk with a round, clear acrylic base devoid of any text. The ZBrush modeling process of the figure is shown on the computer screen. Beside the computer screen, a BANDAl-style toy box printed with the original illustration is positioned` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
