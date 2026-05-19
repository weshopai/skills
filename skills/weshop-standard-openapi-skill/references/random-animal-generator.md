# random-animal-generator (v1.0)

Generate a hyper-realistic wildlife photo of any animal

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | No | Reference image URL (optional) |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | No | Reference image URL (optional); up to 1 |
| `textDescription` | string | No | Describe the desired animal and scene; default `A hyper-realistic, award-winning wildlife photograph of [ANY RANDOM ANIMAL] in its natural habitat. Captured in a National Geographic style to emphasize natural lighting and fur/scale texture. Shot on a Sony A1 with a 600mm f/4 lens for a shallow depth of field and a creamy bokeh background. The composition follows the rule of thirds, showing the animal in a candid, unposed moment—such as hunting, resting, or observing its surroundings. Incredible detail on the eyes, whiskers, and environment, 8k resolution, cinematic atmosphere, sharp focus, natural color grading.` |
| `batchCount` | integer | No | Number of images to generate; default `1`; range `1-16` |
