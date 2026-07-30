# Visual Lens Library

[English](README.md)

フォトリアルな画像生成に使用できる、日英併記の写真表現プロンプト集です。

ここでいう**レンズ**とは、実在する光学レンズの仕様ではなく、被写体から
独立して再利用できる視覚表現の体系です。利用者が被写体、動作、構図、
撮影距離、撮影角度などを指定し、レンズ側が色彩、照明、焦点、光学的な
質感、粒子、空気感、避ける表現を一貫して制御します。

異なる被写体や場面に適用しても、同じ写真世界の一枚として認識できる
状態を目指しています。

## レンズ一覧

| レンズ | English name | 表現の核 | プロンプト |
| --- | --- | --- | --- |
| 水中毛並みレンズ | Underwater Fur Lens | 冷たい青緑の水、砕けた水面光、水を含んだ毛、粗い35mmフィルム | [開く](lenses/underwater-fur-lens.md) |
| 朧げの春 | Hazy Spring Lens | 壊れそうな白緑の春光、水彩のような背景ボケ、小さな対象への選択的な焦点 | [開く](lenses/hazy-spring-lens.md) |
| 凍レンズ | Frozen Lens | ほぼ単色の氷青、圧縮された階調、極細の毛、冷たく親密な静けさ | [開く](lenses/frozen-lens.md) |
| ノスタルジックサマー | Nostalgic Summer Lens | 古い水辺のスナップ、青緑に偏ったカラーネガ、眩しさ、粒子、不完全な動き | [開く](lenses/nostalgic-summer-lens.md) |
| 幻想 | Reverie Lens | 低彩度の深い夜、非対称なハレーション、大胆な逆光の影、天体との偶然の重なり | [開く](lenses/reverie-lens.md) |
| ソフトイエロー | Soft Yellow Lens | 乳白色のハイキー光、控えめなバターイエローと若葉色、選択的な精細さ、美しい白 | [開く](lenses/soft-yellow-lens.md) |
| 夏底 | Summer Depths Lens | 青みを帯びた深緑の木陰、大きな乳白色フレア、粗い植物描写、有機的な35mm粒子 | [開く](lenses/summer-depths-lens.md) |
| 秘密の時間 | Secret Hours Lens | 淡いオレンジを含む桃色の退色、高密度のフィルム粒子、画面全体の甘い焦点、無人の公共空間に残る親密な秘密 | [開く](lenses/secret-hours-lens.md) |
| トイ | Toy Lens | 実物大の玩具めいた遊具、温かな白とシアンブルー、限定的なキャンディ色、実在感のある動物、静かな可笑しさ | [開く](lenses/toy-lens.md) |
| グラスモノクローム | Glass Monochrome Lens | レンズ側のすりガラス状拡散、完全なモノクローム、深い黒のビネット、一点に集めた真珠白の光 | [開く](lenses/glass-monochrome-lens.md) |
| 粉雪 | Powder Snow Lens | 青白いハイキー階調、高密度の微細粒子、穏やかな焦点、唯一残る控えめな赤 | [開く](lenses/powder-snow-lens.md) |

## 使い方

1. 求める空気に近いレンズを開きます。
2. **Primary request**内の角括弧で囲まれた差し替え欄を埋めます。
3. **Focus target**などの追加欄がある場合は、そこも指定します。
4. Style preset、Constraints、Avoidは一組のまま使用します。
5. 完成したプロンプト全体を画像生成モデルへ入力します。
6. レンズ本体を変更する前に、まず場面を指定する変数部分を調整します。

例：

```text
［毛のある動物・動作・撮影距離・撮影角度］

↓

［ボルゾイ・水中で体全体を旋回させ、長い毛が水流に遅れて靡いている・
少し遠い・被写体より浅い場所からわずかに見下ろす］
```

## ファイル構成

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
│   └── powder-snow-lens/
│       ├── english-golden-retriever-basketball.jpeg
│       ├── english-golden-retriever-red-flying-disc.jpeg
│       ├── white-dog-red-shaved-ice.jpeg
│       └── white-shepherd-strawberry.jpeg
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

各レンズのファイルには、次の内容を収録しています。

- 固定メタデータと差し替え可能な入力項目
- 完全な英語版プロンプト
- 対応する日本語原文
- 作例がある場合は、その視覚ギャラリー
- 共通のライセンス表記

## クレジット表記

プロンプトを再配布または改変する場合は、たとえば次のように表記できます。

```text
Visual Lens Library（CC BY 4.0）をもとに改変。
```

可能な場合は「Visual Lens Library」から公開リポジトリへリンクし、
改変の有無を示してください。

## ライセンス

このリポジトリに含まれるプロンプト本文および文書は、
[Creative Commons Attribution 4.0 International License](LICENSE.md)
で公開します。

適切なクレジットを表示し、ライセンスへのリンクと改変の有無を示すことを
条件に、コピー、再配布、改変、翻案、商用利用が可能です。
