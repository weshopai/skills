# see-through-clothes-fitler (v1.0)

Make clothing appear sheer and see-through

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input photo URL; up to 1 |
| `textDescription` | string | No | Custom sheer fabric instruction; default `Change the fabric to a super-thin and sheer material with no color, allowing for faint visibility through it.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
