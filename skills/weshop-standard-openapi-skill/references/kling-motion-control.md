# kling-motion-control (v1.0)

Motion transfer from reference video to character image with Kling Motion Control

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Character reference image URL |
| `input.videos` | array | Yes | Motion reference video URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Character reference image URL; up to 1 |
| `videos` | array | Yes | Motion reference video URL; up to 1 |
| `textDescription` | string | No | Optional prompt to refine background, style, or scene details |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
