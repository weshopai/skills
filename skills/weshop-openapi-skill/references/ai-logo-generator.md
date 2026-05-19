# ai-logo-generator (v1.0)

Design brand logos directly from text descriptions of brand name, industry, and style

## Run parameters

| Field | Type | Required | Notes |
| --- | --- | --- | --- |
| `textDescription` | string | Yes | Describe the brand, industry, style, and visual preferences for the logo; default `Create a clean, professional logo for [BRAND NAME], a [BRAND TYPE/INDUSTRY].
Style: [modern/minimal/luxury/tech/playful].
Include a simple icon or symbol that reflects [CORE IDEA].
Use a strong, memorable, scalable logo design with clean shapes and minimal details.
Background should be simple and uncluttered.
Prefer a vector-style look, balanced composition, and high brand recognizability.` |
| `batchCount` | integer | No | Number of logo variations to generate; default `1`; range `1-16` |
