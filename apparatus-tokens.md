# Apparatus Library — Design Token Reference
> Used by: **6labs** project (Figma file: `i9fxQ6pXrgRITEzopoXpWL`)
> Apparatus file: `Nt21OzTRlJKgvSLMoSxTyT`
> Last updated: 2026-04-03 (live sync from Figma)

---

## Variable Import Method

**Always use `figma.variables.importVariableByKeyAsync(key)`** — never `getVariableByIdAsync`.
Variable IDs are local-only; keys are stable across files.

---

## Component Keys

| Component | Key |
|---|---|
| `Button` (Primary, Default state) | `d4ae660adb3576bfae3c77dda7c2202b47055b6a` |

> Component key extraction is batched per session — re-run `figma.getLocalComponentsAsync()` to enumerate all keys.

---

## Color Tokens — Collection: Colors

### Base Scale

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Base/Base-950` | `de10ac7d76c48a02d9cfed3b90f3fc0b7300403f` | `#080D1A` | Dark mode page bg — deepest |
| `Base/Base-925` | `3f2fa7d382419109a7618b50886faae2af748104` | `#111827` | Dark mode card/surface bg |
| `Base/Base-910` | `9a54a05fc4b5fe4286a55987178c6dfe85d43cc7` | `#1A2236` | Dark mode elevated surface |
| `Base/Base - 900` | `60221769b400401712fdcd7f87622e026d92e2e8` | `#030D2D` | Primary text, headings |
| `Base/Base - 800` | `5b00f6d3ce4bf75bbebbf1739c5de55b42520d0f` | `#1C2542` | Very dark navy |
| `Base/Base - 700` | `261c4c6e156b8d81405f13e4f1495460e07ec55d` | `#353D57` | Dark navy-grey |
| `Base/Base - 600` | `0a2933abde9dd308b926700b71779276b560e4a0` | `#4F566C` | Secondary text (light mode) |
| `Base/Base - 500` | `9def0dd249e14ca795a099b46fca920394664b29` | `#686E81` | Tertiary text, disabled |
| `Base/Base - 400` | `188d3920ef1f79870a90e95f50eee3aa917c3b6c` | `#818696` | Secondary icons, light borders |
| `Base/Base - 300` | `dc95cee51d9749ee6024ca5a4d2c43c95411c431` | `#9A9EAB` | Placeholder, inactive |
| `Base/Base - 200` | `3cd1c141e95f041aabfa6eab5c189d53e8a07d43` | `#B3B6C0` | Pale grey, hover bg |
| `Base/Base - 100` | `82f2b0b969ddf49c97ece9663aecd2a4ff76a68b` | `#CDCFD5` | Card borders, dividers |
| `Base/Base - 50` | `53dee2fa85c343f2f6a263007c38083b75d62479` | `#E6E7EA` | Tag/chip bg, subtle fills |

### Neutral

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Neutral/White` | `3edd2c478ba89189d241ae6f0b3e778b1eb3774b` | `#FFFFFF` | Pure white |
| `Neutral/Black` | `4bf62193d4afca71b0f1f361327d254f8e5a25da` | `#000000` | Pure black |
| `Neutral/Surface` | `bcdcb8daffb9c4d1bd1a12cc31a0e0a70a0bbc26` | `#F1F1F1` | Default card/panel bg |
| `Neutral/Surface-Pale` | `edcf34b84acf4628f8d7b194141802fb6472862f` | `#F5F5F5` | Page bg, section dividers |

### Brand Blue

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Brand Blue/600` | `9d8a3571885f8e6f23763277d7df7172df96c914` | `#0D5ED4` | Primary button pressed |
| `Brand Blue/500` | `8a8916d8f8e4ca58a2bd3197c7b11ebd01713f63` | `#1770EF` | Core brand — CTAs, links, active |
| `Brand Blue/400` | `fa855e1121f6e14c4a9cecdd856cc975f0b9bfbc` | `#4D8FF5` | Hover / dark mode primary |
| `Brand Blue/Tint Dark` | `685a03baaee4c3f3c5530570c0c3c0bc719e84d1` | `#1770EF66` (40%) | Dark bg selected state |
| `Brand Blue/Tint` | `d1a9b4c49e63f4746ac45aeb44cb2aaec3fb09a1` | `#1770EF24` (14%) | Selected bg, focus rings |
| `Brand Blue/Tint Light` | `c19e1b6174c14655a42c9f854f1764473ac7d57d` | `#1770EF12` (7%) | Light hover tint |

### Complementary

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Complimentary/Pink/500` | `7b8bc797c09ee06fb22849331ba3079351d73a58` | `#C20568` | Hot-pink accent CTAs |
| `Complimentary/Pink/400` | `3f21a7ed1998d702d3e85aea6744c81ab9b0d3ad` | `#E31776` | Pink hover |
| `Complimentary/Pink/Tint Light` | `0d5c6abce7b5a242e44ea7d72e0521420e23c5f9` | `#C2056812` | Pink hover tint |
| `Complimentary/Pink/Pink Tint Dark` | `d3f105bc5eeb046855ccf9ce68ee2c10078effd7` | `#C2056866` | Pink dark bg tint |
| `Complimentary/Purple/500` | `f5790114d853bd5bbfa3bde6e9f857fb58633a7e` | `#7B4CFF` | AI features, premium |
| `Complimentary/Purple/400` | `848621a0d6399273e37e1acb752908d0c76e121a` | `#9873FF` | Purple hover |
| `Complimentary/Purple/Tint Light` | `e9ec26ac53bfb6f6508ee1a40593d374ffb43502` | `#7B4CFF12` | Purple hover tint |
| `Complimentary/Purple/Tint Dark` | `8250fbe64d4b363b84a904f0300e200aadd3fbf3` | `#7B4CFF66` | Purple dark bg tint |

### Status

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Status/Error` | `38b180f446c75dc88bba0fd75625025271c88cbd` | `#C9392A` | Error red |
| `Status/Error Dark` | `29c17caca5513ebbc2ce94a111a4529c6787333b` | `#A52E20` | Destructive pressed |
| `Status/Error Light` | `575e5772c9e0e5f7d4cac3659ed5b807993be5f0` | `#DE5A48` | Error hover on dark |
| `Status/Error Tint Light` | `f4997f68cff1c4a2a1e06c1b4075c0ca2f13930e` | `#C9392A12` | Error bg fill |
| `Status/Error Tint Dark` | `4e3def175c4a33d9b81baef97a93420eab15d292` | `#C9392A66` | Error dark bg fill |
| `Status/Warning` | `737cf72094488e099cea340e89fcd68a31ad2999` | `#FFB700` | Warning amber |
| `Status/Warning Tint Light` | `652e2ee4a18759110fc22145c7f8302204f699f2` | `#FFB70012` | Warning bg fill |
| `Status/Success` | `c053dc86923bfc19b7894000e0be6aa9ae6eebcb` | `#16A34A` | Success green |
| `Status/Success Tint Light` | `1a0263993c3edfaef2ee97e265ad04377bef1fc0` | `#16A34A12` | Success bg fill |
| `Status/Notice` | `a1456e6319fe18823dcff48396098c7047d58170` | `#67C3BB` | Teal — informational |
| `Status/Notice Tint Light` | `f719b27da1667e4941a384682c9b1d2ad2cf8a97` | `#67C3BB12` | Notice bg fill |

### Translucents

| Token Name | Key | Resolved Value |
|---|---|---|
| `Translucents Dark/Black-4` | `aba6fcafd6c5303f44f75c1623fc5e5725123d9f` | `#0000000A` |
| `Translucents Dark/Black-8` | `9f284ed4a660d0e625c2f66bd8fb142c3db38220` | `#00000014` |
| `Translucents Dark/Black-10` | `288cd30af982253143df03a8f267af6f9eff356e` | `#0000001A` |
| `Translucents Dark/Black-16` | `cf668f44a6e6fcb837ca73eadd2547804e82acb5` | `#00000029` |
| `Translucents Dark/Black-20` | `cc4722d19c495215ff0d0a33cc112b8dec3c954c` | `#00000033` |
| `Translucents Dark/Black-30` | `4521bf43124d156e31437a26a3d9e5dc826e35cc` | `#0000004D` |
| `Translucents Dark/Black-40` | `4a7d56da1e1039b8f5047d402e080967ed5d1750` | `#00000066` |
| `Translucents Dark/Black-50` | `59650bbd2cb03674671cb6f44c24b2a21868974c` | `#00000080` |
| `Translucents Dark/Black-60` | `2d1be99b7339e7b4a236c38fb20a3bdb7eae813b` | `#00000099` |
| `Translucents Dark/Black-70` | `01e90fe0725a5f2b3459b7b6b27d420f6298c40c` | `#000000B2` |
| `Translucents Dark/Black-80` | `d6bc0c92a9370e6ff2f9d3c5fbea00aac11d1ec3` | `#000000CC` |
| `Translucents Dark/Black-90` | `78239f1a57cc4712c07c9609c3588bee123f455c` | `#000000E5` |
| `Translucents Light/White-10` | `73c53ad1323ef1b1fb0d2873ade09639f846cb32` | `#FFFFFF1A` |
| `Translucents Light/White-12` | `de40e7c03c4363486396b52ad3cac61792eb57ca` | `#FFFFFF1F` |
| `Translucents Light/White-20` | `2729661918b524af43c27c248cdc8d8fd431f245` | `#FFFFFF33` |
| `Translucents Light/White-25` | `6009592db0cd39c119c2e3e17a4fee604b2ba085` | `#FFFFFF40` |
| `Translucents Light/White-30` | `92b424a3c17456e903f5bf86b47785b9ff59d1bf` | `#FFFFFF4D` |
| `Translucents Light/White-40` | `8c7a45e32574fc56019b4db0b3b649d34b8eb5ae` | `#FFFFFF66` |
| `Translucents Light/White-50` | `8caea6d689690240cd92a292364be34d158f20fa` | `#FFFFFF80` |
| `Translucents Light/White-60` | `943c852f310e20781d52d45064d1d92978dabf8a` | `#FFFFFF99` |
| `Translucents Light/White-70` | `f2f328786daef900fbb7be087947b44dfe291dc6` | `#FFFFFFB2` |
| `Translucents Light/White-80` | `53ee223a3d10dbaa48ee3c931f4004275fbbdc2a` | `#FFFFFFCC` |
| `Translucents Light/White-90` | `6158357f03ce9512361f2b6f2818b380287b5baa` | `#FFFFFFE5` |

---

## Semantic Tokens — Collection: Semantic (Light / Dark modes)

> Resolved values shown as Light → Dark. These alias primitive tokens.

### Background

| Token Name | Key | Light | Dark |
|---|---|---|---|
| `Background/Elements` | `146ff989c79525dc33c46c338611c9f8b40a52f4` | `#FFFFFF` | `#080D1A` |
| `Background/Card` | `2910233d5d0171d23b8e6f013430570c0bf9896e` | `#FFFFFF` | `#111827` |
| `Background/Page BG` | `9cf5e54da014b68dd50661539f573eddd9b359e9` | `#F1F1F1` | `#1A2236` |
| `Background/ALT Page BG` | `c9b03102055b8e5d3498311bba13088a478e89b8` | `#F5F5F5` | `#1A2236` |
| `Background/Subtle` | `389caeb17542d338f31bdc962d025d71da5fc3f3` | `#E6E7EA` | `#1C2542` |
| `Background/Highlighted` | `72e4fc9a8b09f16e3855b44e599c68504142355b` | `#1770EF` | `#1770EF` |
| `Background/Highlighted Tint` | `da3e23a95731e2bd9b8b8f18c99c72156ff84ee5` | `#1770EF24` | `#1770EF24` |
| `Background/Highlighted Tint Light` | `48aa3d4bdad4f90f6a91c5b357f2400d09c8b347` | `#1770EF12` | `#1770EF12` |
| `Background/Highlighted Tint Dark` | `6d35851e573fe6381266e145380dd2b26b86f529` | `#1770EF66` | `#1770EF66` |

### Text & Icon

| Token Name | Key | Light | Dark |
|---|---|---|---|
| `Text & Icon/Primary` | `5bcb5ca00dd06c96b703c88189f80ebc8a520748` | `#030D2D` | `#FFFFFF` |
| `Text & Icon/Secondary` | `c9cf7517427eed7f8d38e075493b0010125ab10c` | `#4F566C` | `#9A9EAB` |
| `Text & Icon/Tertiary` | `6b879b88984e250c0742d2c35f45ca69654ad83d` | `#818696` | `#686E81` |
| `Text & Icon/Placeholder` | `6a11e16d641885efe501f31178b18f97012cb979` | `#9A9EAB` | `#686E81` |
| `Text & Icon/Disabled` | `0626506f38d7a3c68b18880930015a7d892996f3` | `#9A9EAB` | `#4F566C` |
| `Text & Icon/OnBrand` | `74864f95dfe7065b74e9da5832662365b86a9170` | `#FFFFFF` | `#FFFFFF` |
| `Text & Icon/OnDark` | `f9120e3b7cdb03005de1f6c7e665fedb088c42bc` | `#FFFFFF` | `#FFFFFF` |
| `Text & Icon/Brand` | `029b55af59d7b919c8b1d7192bb396793f224dfe` | `#1770EF` | `#1770EF` |

### Border

| Token Name | Key | Light | Dark |
|---|---|---|---|
| `Border/Default` | `80e69d28b62fd63385657c7eaa1f435c2a00e8af` | `#CDCFD5` | `rgba(255,255,255,0.12)` |
| `Border/Hover` | `e99cb844f3ebd39643a10590d0aa2a497d623564` | `#9A9EAB` | `rgba(255,255,255,0.25)` |
| `Border/Focus` | `77eee1910044597fba0971d35cb8db4262b25414` | `#1770EF` | `#4D8FF5` |
| `Border/Error` | `7810d4e2af199f40924a37771f2660644b5c90b1` | `#C9392A` | `#C9392A` |
| `Border/Subtle` | `ec9335d574d992971305e05f5888967b917816ce` | `#E6E7EA` | `rgba(255,255,255,0.06)` |
| `Border/Tint` | `cf5ddadc3f78249005768b63cd32c8a3ea739cef` | `#1770EF24` | `#1770EF24` |
| `Border/Tint Light` | `536500461da06e860eb578270c3d8e497d54362c` | `#1770EF12` | `#1770EF12` |
| `Border/Tint Light Dark` | `2b2133538868fe0dca3a89528fa6cfe7a85a012a` | `#1770EF66` | `#1770EF66` |
| `Border/Brand Hover` | `b3ec71fd06afde3e0e7086713a71c09950618f14` | `#4D8FF5` | `#4D8FF5` |

### Interactive

| Token Name | Key | Value |
|---|---|---|
| `Interactive/Brand` | `638439cce82a651f0a44efaa97d8e2f4662fce38` | `#1770EF` |
| `Interactive/BrandHover` | `f4c46365fce817add782eed28fbd39c25af528d1` | `#4D8FF5` |
| `Interactive/BrandPressed` | `9df5fef7f0a67bb588a87ed3ea69bd138aa8ad40` | `#0D5ED4` |
| `Interactive/BrandFocusRing` | `2e22d92d1ab36a55696e98830584ba9ef5aeb5e1` | `#1770EF` |

---

## Spacing Tokens — Collection: Spacings

| Token Name | Key | Value |
|---|---|---|
| `Null` | `aad3b7f70969bb1d4adc403acabdb76a4316b653` | `0px` |
| `xxxs` | `a2f10eb3e142494b6377df38e6be9adc9b131eea` | `2px` |
| `xxs` | `fc99050b5f5c043fa5fb56f4b92586afeff3a1fb` | `4px` |
| `xs` | `707e5d30518900d7af474e49ab5cb76a1822d3a5` | `8px` |
| `s` | `a3e66a8a7e7b61907cca0ab0400021cbad31c85a` | `12px` |
| `m` | `4ebbaf8831b7d71ba70c6377630bf5eca7a367b2` | `16px` |
| `l` | `b70e08177755d675ac8670d81f0fa33ae02026ee` | `20px` |
| `xl` | `6636794aecbb6cbdb4dd47f16a93dc3fb1e45d31` | `24px` |
| `xxl` | `561281161554efc974a87c40bfd7e0a6c72bd99a` | `32px` |
| `xxxl` | `6a6f1912452c4964fe689826bd4e14885e33a47f` | `40px` |
| `xxl2` | `64f5611c60afc5a1bcbf78a0556b66e4f0150200` | `48px` |
| `xxl3` | `57def1b9e14e2cd35cff4a4154c3c6ae334e59d9` | `64px` |
| `xxl4` | `ae9788bbe917cceb2ef2d126ff1999200d771981` | `80px` |
| `xxl5` | `adb1d721ad00d594f3b07ba2bcd50aa8db7022b4` | `96px` |

---

## Border Radius Tokens — Collection: Radius

| Token Name | Key | Value |
|---|---|---|
| `null` | `8b62226e63478e8cc364b67d739bf04aa6e3777d` | `0px` |
| `xxs` | `0ce57cd99ac18691262430345a3d5c442e8a0ed7` | `2px` |
| `xs` | `d65d1a6b269344cfee77611f3ff36c1fd968fdc1` | `4px` |
| `s` | `c96d6121fb4ba2c883b1108d7fc1ead8b1d1b625` | `6px` |
| `m` | `4b4bbcd8bf2e190a853ebe5ca9f166bc9ae6a6ac` | `8px` |
| `l` | `71987574f6893a8aecb1aea19136366eb9c973ea` | `10px` |
| `xl` | `4c8e24357cff5aed1f0b875fb8b354fb4e1c212c` | `12px` |
| `2xl` | `17dbe0797b122cc530f0e3f0f1e3010e18c66f5c` | `16px` |
| `3xl` | `daa4ffcd155d09784e1754b73fad90f59fef87b4` | `20px` |
| `4xl` | `827a43e704caa2f475df490aadbfc04917c24168` | `24px` |
| `5xl` | `d257c9b5a2e6edb8f362457045c88bdfaad62fec` | `32px` |
| `6xl` | `f30811d70957657ab6772ffc44815c89867b89c1` | `40px` |
| `Round` | `266569fe96c015e595be7ebf0626f5e92c0b7843` | `9999px` |
| `Semantic/button/small` | `33125825fdeca5bc2408857a654f77618aa69981` | `4px` (→ xs) |
| `Semantic/button/medium` | `5ef3e7dfc9e71fe41c11ceffd0cfc317ee281403` | `6px` (→ s) |
| `Semantic/button/large` | `2a213f054cab3d56156be00a04af0b49185ed5a0` | `8px` (→ m) |
| `Semantic/button/xlarge` | `54bea48dc2e7af7dbd594a8580c697505bc2a1fa` | `10px` (→ l) |
| `Semantic/button/Pill` | `bc0f51539acf65121ef299d1c0799bb4a44f8035` | `9999px` (→ Round) |
| `Semantic/input` | `c26b648a2825666c2ed8aecc1965cd92ea375e62` | `6px` (→ s) |
| `Semantic/card` | `95b3aed26816b19f1f2dfe4427aea657890beb73` | `12px` (→ xl) |
| `Semantic/modal` | `3c000fd64b5b15b815a79703031a115b87f417f1` | `8px` (→ m) |
| `Semantic/tag` | `2df037d0ecf00024087e4f0ab8e947d7ea38ced2` | `4px` (→ xs) |
| `Semantic/avatar` | `8b5ce9e32f8e3e77dfd38bb722b447fea7704c9b` | `9999px` (→ Round) |
| `Semantic/tooltip` | `4141349c438de9b5dff479aa6d34bbe7d09470e9` | `4px` (→ xs) |
| `Semantic/Container` | `ce0eda81136e73de64572b79314e48d939ada7bd` | alias → check live |

---

## Typography Tokens — Collection: Typography

### Font Families

| Token Name | Key | Value |
|---|---|---|
| `DisplayFont` | `a7f0f012dae7643096ff6d77e7b7cfdde19b320e` | `Bricolage Grotesque` |
| `BodyFont` | `88232b013efe0b35810d624c9b306704a60eb77e` | `Inter` |
| `CompactFont` | `301404cf54be368ffb3fcf78b5bace682394dea3` | `Roboto Mono` |

### Font Sizes (Default mode)

| Token Name | Key | Default | Compact |
|---|---|---|---|
| `size/2xs` | `798691c2357f4c5d4aed8c70439ccc76e6c9e220` | `10px` | — |
| `size/xs` | `2d2ce76c53d63653935f83f89ac9118b92c371b8` | `12px` | — |
| `size/s` | `37a60de618cb2058efa6a0e43377f2bc98cedc91` | `14px` | — |
| `size/m` | `98547d8c5f864ea460160ed3faeaf7002bbbf982` | `16px` | — |
| `size/l` | `aa5debc1bef09591d166a065f3051a9dbccf5bb2` | `20px` | — |
| `size/xl` | `575448093bceb106e21356fe714ef0c7030a9f1e` | `24px` | — |
| `size/2xl` | `74bb7bb9b0d637fc71bb67f8f40a7b072958902b` | `32px` | — |
| `size/3xl` | `abfb7714033539e6bb3cde0fce009fba3c0393e9` | `36px` | — |
| `size/4xl` | `3bab46a795641188ebd84a2c9a4a21f97e1fdb89` | `48px` | — |
| `size/5xl` | `39f02eb04e18f38c3d6585333a2f0fec9c165c70` | `64px` | — |

### Font Weights

| Token Name | Key | Value |
|---|---|---|
| `weight/regular` | `029e5cc3ca4b77edcfca1e34cfe5d7b32dccd857` | `400` |
| `weight/medium` | `df5d7fac7bf91c31682ab7aade965576e0904bce` | `500` |
| `weight/semibold` | `82bb8269c04227bf5da1934884e7b69bfe29daa7` | `600` |
| `weight/bold` | `be2e3cf50e599010acfed5a589f8bf718c03b061` | `700` |
| `weight/extrabold` | `1cdf033bab22b0a8ae4bece7d1574c5d22658894` | `800` |

---

## Text Styles

| Style Name | Key | Size | Family | Weight | Line Height |
|---|---|---|---|---|---|
| `Title/5XL` | `e4bad7f98b8e88fa41ead9c2b37416686bdf9df6` | 64px | Bricolage Grotesque | Bold | 110% |
| `Title/4XL/ExtraBold` | `45bf2d61b653e95d71e6595644febe7319d2dd00` | 48px | Bricolage Grotesque | 96pt ExtraBold | 120% |
| `Title/4XL/Semibold` | `1ef62648c307ad9df4873405955c71ee11c13558` | 48px | Bricolage Grotesque | SemiBold | 120% |
| `Title/3XL/Bold` | `6c606dcbc71e0127908f086c166c166760b35c69` | 36px | Bricolage Grotesque | 96pt ExtraBold | 150% |
| `Title/3XL/Medium` | `928f536810e1434bf5141b1665556eb78128f1ad` | 36px | Bricolage Grotesque | Medium | 150% |
| `Title/3XL/Regular` | `2674185bcd2731ebd727322b172543f233ac9762` | 36px | Bricolage Grotesque | Regular | 150% |
| `Title/2XL/Bold` | `0617f2f5e32ba1ffef90451fd4c833dc3fa7f10c` | 32px | Bricolage Grotesque | 96pt ExtraBold | 150% |
| `Title/2XL/Medium` | `15bc86ee0ca7c4530fe23f9ba82a2ad115ab6987` | 32px | Bricolage Grotesque | Medium | 150% |
| `Title/2XL/Regular` | `21cf8ac6e1b5c9cff788d8ebf392c65919673162` | 32px | Bricolage Grotesque | Regular | 150% |
| `Title/XL/Medium` | `7d7ccd824d2b4b1f4a5027cedde6af27fbbc2cef` | 24px | Bricolage Grotesque | Medium | 150% |
| `Title/XL/Regular` | `c8df693321b4687de92facc0049d01e071e70ba5` | 24px | Bricolage Grotesque | Regular | 150% |
| `Title/XL/CAPS` | `bd8508266276c32cdc8baf153130f089100129ff` | 24px | Bricolage Grotesque | Bold | 130% UPPER |
| `Title/L/Medium` | `b3a77475c0d0fde48b845f6aebcc15a0468d22d5` | 20px | Bricolage Grotesque | Medium | 150% |
| `Title/L/Regular` | `9d88a699bc19a2f658fb34ae6383357315751f3e` | 20px | Bricolage Grotesque | Regular | 150% |
| `Title/L/Caps` | `168ba588d9bff47aaf986cb295106b4d9cad8d1d` | 20px | Bricolage Grotesque | Bold | 130% UPPER |
| `Title/M/Semibold` | `10148b472f1d17976dfbd71c7be063ce5387abdb` | 16px | Bricolage Grotesque | SemiBold | 150% |
| `Title/M/Bold` | `33e696f137f56bd2764f371797deef96c7b55b47` | 16px | Bricolage Grotesque | Bold | 150% |
| `Title/S/Semibold` | `0287e7bac372c79f78329abbe3fec929d2725ef3` | 14px | Bricolage Grotesque | SemiBold | 150% |
| `Title/S/Bold` | `a477a6cc0f97f592e11bc7342d7b3e42e1fe11b4` | 14px | Bricolage Grotesque | Bold | 150% |
| `Title/XS/Semibold` | `c73531ac20c0d1b20f391f72666cf42bc33c8afc` | 12px | Bricolage Grotesque | SemiBold | 150% |
| `Title/XS/Bold` | `3761c2a1f334f976175f973dfd3912399dca71f9` | 12px | Bricolage Grotesque | Bold | 150% |
| `Body/L/Regular` | `19d76320f08898057faf6fea12c0205ef6327171` | 16px | Inter | Regular | 150% |
| `Body/L/Medium` | `1535ee4237762c71eed4a290f7cfa2ffb9bed9ed` | 16px | Inter | Medium | 150% |
| `Body/L/Semibold` | `4eacf73cf12d069eeecec7de277b9807d3cf6709` | 16px | Inter | Semi Bold | 150% |
| `Body/M/Regular` | `be436272959918060d24b6f06c494051cc047502` | 14px | Inter | Regular | 150% |
| `Body/M/Medium` | `569ce5fee3945ea1d4bfd38964bfe4967a8aa569` | 14px | Inter | Medium | 150% |
| `Body/M/Semibold` | `fc2207d57c8890d6630cc41d462e04ffe9f1b861` | 14px | Inter | Semi Bold | 150% |
| `Body/M/Underlined` | `5d25c508d9017183618e79bdbd52677088be9712` | 14px | Inter | Regular | 150% |
| `Body/S/Regular` | `be2440d7bde42d0cc7639c68a5e9031b5178e6fa` | 12px | Inter | Regular | 150% |
| `Body/S/Medium` | `a97c25ae1411d33d07d01b9260838f565e7ffdfe` | 12px | Inter | Medium | 150% |
| `Body/S/Underlined` | `a3a02db173f7322b85bad1b1ec9e1f5c7d368612` | 12px | Inter | Regular | 150% |
| `Body/S/Graph Legend` | `8c5620ffed43cff2d69b3dd3bab177846aed697b` | 12px | Inter | Regular | 100% |
| `Body/XS/Regular` | `b526359ce8f3e57f9b3c93a729b807cf6651dd67` | 10px | Inter | Regular | auto, 2% ls |
| `Body/XS/Medium` | `0082a0c0a6c72d4381db8ca491dd8a675e886ea8` | 10px | Inter | Medium | 16px, 2% ls |
| `Label/Medium` | `15e7949495398034edf6a48b0a180c838c1d188d` | 10px | Bricolage Grotesque | Medium | auto, 15% ls UPPER |
| `Label/Regular` | `15841e0c026639e5b0760b07a7ab93625159aa66` | 10px | Bricolage Grotesque | Regular | auto, 14% ls UPPER |
| `Button Label/Small` | `1a156d9fd23a95badf2273260be7adaf8b65ba48` | 10px | Bricolage Grotesque | SemiBold | 16px |
| `Button Label/Medium` | `d357426d3e9e06a9a717fa67943352dc14902fd1` | 12px | Bricolage Grotesque | SemiBold | 16px |
| `Button Label/Large` | `12014a6db66ab7a6c974db3e6811efaab63dfde9` | 14px | Bricolage Grotesque | SemiBold | 20px |
| `Button Label/XLarge` | `1ff7b607581c4c6c2d2525d6b93123134418acaf` | 16px | Bricolage Grotesque | SemiBold | 24px |
| `Code/Regular` | `9b463c350f78be8fd5fe93ab9f5dc70820fe5047` | 12px | Roboto Mono | Regular | 150% |
| `Code/Small` | `7435cbc1a881a34718217e6f9f5158d07ec10fd1` | 11px | Roboto Mono | Regular | 150% |
