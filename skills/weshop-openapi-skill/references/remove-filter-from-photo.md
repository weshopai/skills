# remove-filter-from-photo (v1.0)

Remove photo filters and restore natural image colors

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Input filtered photo URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Input filtered photo URL (optional); up to 1 |
| `textDescription` | string | No | Describe the filter to remove; default `Remove [any style] filter you think this photo have, including b&w filter.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
