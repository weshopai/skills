# aipose (v1.0)

Change the human pose while preserving the garment.

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.originalImage` | string(url) | Yes | Publicly reachable source image URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `textDescription` | string | Yes | Pose instruction |
| `generateVersion` | string | No | `lite` or `pro`, default `lite` |
| `batchCount` | int | No | Range `1-16`, default `4` |
