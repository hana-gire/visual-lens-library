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
| Secret Hours Lens | 秘密の時間 | Faded peach-pink light, dense old-film grain, uniformly soft focus, intimate encounters in empty public spaces | [Open](lenses/secret-hours-lens.md) |
| Toy Lens | トイ | Life-size toy-like rides, warm white and cyan blue, restrained candy accents, photoreal animals, quiet visual absurdity | [Open](lenses/toy-lens.md) |
| Glass Monochrome Lens | グラスモノクローム | Lens-side frosted-glass diffusion, strict monochrome, deep black vignette, one concentrated pearl-white highlight | [Open](lenses/glass-monochrome-lens.md) |
| Powder Snow Lens | 粉雪 | Pale blue-white high-key tonality, dense fine grain, gentle focus, one restrained red accent | [Open](lenses/powder-snow-lens.md) |

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
├── examples/
│   ├── frozen-lens/
│   │   ├── borzoi-in-snow.jpeg
│   │   ├── penguin-chick-sleeping.jpeg
│   │   ├── polar-bear-over-shoulder.jpeg
│   │   ├── polar-bear-underwater.jpeg
│   │   ├── polar-bears-sleeping.jpeg
│   │   ├── samoyed-stargazing.jpeg
│   │   └── swan-water-splash.jpeg
│   ├── glass-monochrome-lens/
│   │   ├── borzoi-phone-booth.jpeg
│   │   ├── camel-in-desert.jpeg
│   │   └── polar-bear-steaming-cup.jpeg
│   ├── hazy-spring-lens/
│   │   └── golden-retriever-blossom.jpeg
│   ├── nostalgic-summer-lens/
│   │   ├── golden-retriever-flying-disc.jpeg
│   │   ├── golden-retriever-shaking-water.jpeg
│   │   └── golden-retriever-shallows.jpeg
│   ├── powder-snow-lens/
│   │   ├── english-golden-retriever-basketball.jpeg
│   │   ├── english-golden-retriever-red-flying-disc.jpeg
│   │   ├── white-dog-red-shaved-ice.jpeg
│   │   └── white-shepherd-strawberry.jpeg
│   ├── reverie-lens/
│   │   ├── golden-retriever-moon-jump.jpeg
│   │   └── golden-retriever-starlight.jpeg
│   ├── secret-hours-lens/
│   │   ├── golden-retriever-deer-sculpture.jpeg
│   │   └── golden-retriever-swan-boat.jpeg
│   ├── soft-yellow-lens/
│   │   ├── great-egret-yellow-flowers.jpeg
│   │   ├── sleeping-white-rabbit.jpeg
│   │   ├── snail-on-leaf.jpeg
│   │   ├── white-seashell-sand.jpeg
│   │   └── white-wagtail-blue-flowers.jpeg
│   ├── summer-depths-lens/
│   │   ├── crow-foraging-refuse.jpeg
│   │   └── raccoon-looking-back-undergrowth.jpeg
│   ├── toy-lens/
│   │   ├── carousel-horse.jpeg
│   │   └── polar-bear-ferris-wheel.jpeg
│   └── underwater-fur-lens/
│       ├── border-collie-dive.jpeg
│       ├── borzoi-surface.jpeg
│       ├── english-golden-retriever-camera.jpeg
│       ├── english-golden-retriever-close-up.jpeg
│       ├── english-golden-retriever-fish.jpeg
│       ├── english-golden-retriever-sideways.jpeg
│       ├── english-golden-retriever-statue.jpeg
│       └── english-golden-retriever-turning.jpeg
└── lenses/
    ├── underwater-fur-lens.md
    ├── hazy-spring-lens.md
    ├── frozen-lens.md
    ├── nostalgic-summer-lens.md
    ├── reverie-lens.md
    ├── soft-yellow-lens.md
    ├── summer-depths-lens.md
    ├── secret-hours-lens.md
    ├── toy-lens.md
    ├── glass-monochrome-lens.md
    └── powder-snow-lens.md
```

Each Lens file contains:

- stable metadata and interchangeable input fields;
- a complete English prompt;
- the corresponding Japanese source prompt;
- where provided, a gallery of visual examples;
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
