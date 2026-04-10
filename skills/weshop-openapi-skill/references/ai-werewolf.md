# ai-werewolf (v1.0)

Create a dramatic werewolf transformation video from a person photo

## Input fields

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `input.images` | array | Yes | Input person photo URL |

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `images` | array | Yes | Input person photo URL; up to 1 |
| `textDescription` | string | No | Describe the werewolf transformation scene; default `The character in the image suddenly begins a violent werewolf transformation. Muscles rapidly expand, veins bulge under the skin. The character roars in pain as their clothes tear apart from the expanding body. Dark fur quickly grows across the arms, chest, and face, covering the body as the transformation continues. Hands stretch and twist into sharp claws, fingers elongating. The jaw extends into a wolf-like muzzle, teeth sharpening into fangs. Eyes glow with a wild golden light. The camera slowly circles the character as the transformation intensifies, pieces of torn clothing flying through the air. By the end, a full ferocious werewolf stands where the human once was, breathing heavily, surrounded by drifting fabric fragments. cinematic lighting, dramatic shadows, dark fantasy atmosphere, high detail, dynamic motion, 4K.` |
| `modelName` | string | No | Kling model: Kling_3_0 (default) or Kling_2_6; `Kling_3_0`, `Kling_2_6`; default `Kling_3_0` |
| `duration` | string | No | Video duration, e.g. 5s, 10s (Kling_3_0: 3s-15s, Kling_2_6: 5s or 10s); default `5s` |
| `generateAudio` | string | No | Generate audio: true (default) or false; `true`, `false`; default `true` |
| `batchCount` | integer | No | Number of videos to generate; default `1`; range `1-16` |
