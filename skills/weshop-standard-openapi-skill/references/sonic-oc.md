# sonic-oc (v1.0)

Create a Sonic the Hedgehog original character based on a person's appearance

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference person image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference person image URL (optional); up to 1 |
| `textDescription` | string | No | Custom Sonic OC description; default `Make a sonic oc based on this person's appearance` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
