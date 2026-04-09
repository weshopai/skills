# Enum Value Reference

Definitions for enum parameters used by various agents. Not all agents use all enums — check each agent's reference file for which parameters apply.

## What the mask means

The mask defines the **protected region**. The AI keeps elements inside the masked area unchanged. Everything outside the mask is the editable region where new content is generated.

## `maskType`

| Enum | Protected region | Effect |
| --- | --- | --- |
| `autoApparelSegment` | Full-body apparel (top + bottom) | Clothing preserved; model face, body, background replaced |
| `autoUpperApparelSegment` | Upper-body apparel only | Top garment preserved; lower body, face, background replaced |
| `autoLowerApparelSegment` | Lower-body apparel only | Bottom garment preserved; upper body, face, background replaced |
| `autoSubjectSegment` | Foreground subject | Subject preserved; only background replaced |
| `autoHumanSegment` | Human body + background | Only face/head editable; for face-swapping |
| `inverseAutoHumanSegment` | Face/head area only | Body and background editable; for outfit replacement |
| `custom` | Caller-defined region | Full manual control |

## `customMask` and `customMaskUrl`

When `maskType=custom`:

- Provide one of `customMask` or `customMaskUrl`.
- `customMask`: base64-encoded PNG without the `data:image/png;base64,` prefix.
- `customMaskUrl`: publicly accessible PNG image URL.
- Dimensions should match the original image.
- Regions outside the selected mask should be transparent.

## `generatedContent`

| Enum | Meaning |
| --- | --- |
| `freeCreation` | Freer generation, less constrained by source style |
| `referToOrigin` | More strongly aligned with source image style |

## `descriptionType`

| Enum | Meaning | Rule |
| --- | --- | --- |
| `custom` | Caller provides prompt text | `textDescription` required |
| `auto` | System generates the prompt | `textDescription` optional |

## `batchCount`

How many result images to generate in one run. Integer, range `1-16`, default `4`.
