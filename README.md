# Visual Lens Library

[日本語](README.ja.md)

A bilingual collection of reusable photographic-style prompt presets for
photorealistic image generation.

Each **Lens** separates visual direction from subject matter. You provide the
subject, action, composition, camera distance, or camera angle; the selected
Lens supplies a consistent photographic grammar for color, light, focus,
optics, texture, atmosphere, and negative constraints.

These are not literal camera-lens specifications. They are named visual systems
designed to preserve a recognizable photographic mood across different
subjects and scenes.

## Lens catalog

| Lens | Japanese name | Visual signature | Prompt |
| --- | --- | --- | --- |
| Underwater Fur Lens | 水中毛並みレンズ | Cold blue-green water, shattered surface light, waterlogged fur, coarse 35mm texture | [Open](lenses/underwater-fur-lens.md) |
| Hazy Spring Lens | 朧げの春 | Fragile green-white spring light, watercolor-like background blur, selective macro focus | [Open](lenses/hazy-spring-lens.md) |
| Frozen Lens | 凍レンズ | Near-monochromatic ice blue, compressed tonal depth, filament-fine fur, intimate stillness | [Open](lenses/frozen-lens.md) |
| Nostalgic Summer Lens | ノスタルジックサマー | Aged waterside snapshot, blue-green color-negative cast, glare, grain, and imperfect motion | [Open](lenses/nostalgic-summer-lens.md) |
| Reverie Lens | 幻想 | Deep low-saturation night, asymmetrical halation, bold backlit shadows, accidental celestial alignment | [Open](lenses/reverie-lens.md) |
| Soft Yellow Lens | ソフトイエロー | Milky high-key light, restrained butter yellow and new-leaf green, selective detail, delicate whites | [Open](lenses/soft-yellow-lens.md) |
| Summer Depths Lens | 夏底 | Deep bluish-green shade, broad milky flare, coarse vegetation, organic 35mm grain | [Open](lenses/summer-depths-lens.md) |

## How to use a Lens

1. Open the Lens that matches the desired atmosphere.
2. Replace the bracketed fields in **Primary request**.
3. Where present, also replace fields such as **Focus target**.
4. Keep the style preset, constraints, and avoid list together.
5. Paste the complete prompt into an image-generation model.
6. Refine the variable scene description before changing the Lens itself.

Example:

```text
[animal with fur — action — camera distance — camera angle]

becomes

[a Borzoi — turning its entire body underwater as its long coat follows the
current — medium-long shot — viewed slightly downward from shallower water]
```

## Repository structure

```text
visual-lens-library/
├── README.md
├── README.ja.md
├── LICENSE.md
└── lenses/
    ├── underwater-fur-lens.md
    ├── hazy-spring-lens.md
    ├── frozen-lens.md
    ├── nostalgic-summer-lens.md
    ├── reverie-lens.md
    ├── soft-yellow-lens.md
    └── summer-depths-lens.md
```

Each Lens file contains:

- stable metadata and interchangeable input fields;
- a complete English prompt;
- the corresponding Japanese source prompt;
- the same permissive licensing notice.

## Attribution

When redistributing or adapting these prompts, a simple attribution may look
like this:

```text
Based on Visual Lens Library, licensed under CC BY 4.0. Modified from the
original.
```

When possible, link “Visual Lens Library” to the public repository and indicate
whether you changed the material.

## License

The prompt text and documentation in this repository are licensed under the
[Creative Commons Attribution 4.0 International License](LICENSE.md).

You may copy, redistribute, remix, transform, and build upon the material for
any purpose, including commercial use, provided that you give appropriate
credit, link to the license, and indicate whether changes were made.
