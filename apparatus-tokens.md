# Apparatus Library — Design Token Reference
> Used by: **6labs** project (Figma file: `i9fxQ6pXrgRITEzopoXpWL`)
> Apparatus file: `Nt21OzTRlJKgvSLMoSxTyT`
> Last updated: 2026-04-09 (token audit: naming fixes, added .Button Tokens + .Forms collections, 304 total vars)

---

## Variable Import Method

**Always use `figma.variables.importVariableByKeyAsync(key)`** — never `getVariableByIdAsync`.
Variable IDs are local-only; keys are stable across files.

---

## Component Keys

### Button (`COMPONENT_SET` id: `12943:1310`)

| Component / Variant | Key |
|---|---|
| `Button` set | import via `importComponentSetByKeyAsync` |
| `Button` (Primary, Default — `Size=Medium, Style=Label & Rounded`) | `d4ae660adb3576bfae3c77dda7c2202b47055b6a` |
| `Button Attributes` set (`id: 12945:1352`) | 16 variants: `Size` × `Style` |
| `Button Attributes` — Small, Label & Rounded | `12943:1292` |
| `Button Attributes` — Medium, Label & Rounded | `12945:1373` |
| `Button Attributes` — Large, Label & Rounded | `12946:1410` |
| `Button Attributes` — XLarge, Label & Rounded | `12946:1428` |
| `Tooltips` set (`id: 12454:3025`) | 4 variants |

**Button component properties:**

| Property | Located On | Type | Default | Options |
|---|---|---|---|---|
| `Type` | `Button` | Variant | `Primary` | Primary · Secondary · Tertiary · Outline · Translucent · Transparent · Link-0-padding · Blueish · Danger · Outline - Complimentary |
| `State` | `Button` | Variant | `Default` | Default · Hover · Click · Disabled · Focus |
| `Size` | `Button Attributes` | Variant | `Medium` | Small · Medium · Large · XLarge |
| `Style` | `Button Attributes` | Variant | `Label & Rounded` | Label & Rounded · Label & Pill · Icon Btn Square · Icon Btn Round |
| `L Icon` | `Button Attributes` | Boolean | `false` | Toggles left icon slot |
| `R Icon` | `Button Attributes` | Boolean | `false` | Toggles right icon slot |
| `Hover Tooltip` | `Button` | Boolean | `false` | Shows hover tooltip |
| `Click Tooltip` | `Button` | Boolean | `false` | Shows click tooltip |
| `Btn Label` | `Button Attributes` | Text | `"Label"` | Button label text |

> Component key extraction is batched per session — re-run `figma.getLocalComponentsAsync()` to enumerate all keys.

---

## Color Tokens — Collection: Colors (mode: Default)

### Base Scale

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Base/Base-950` | `de10ac7d76c48a02d9cfed3b90f3fc0b7300403f` | `#080D1A` | Dark mode page bg — deepest |
| `Base/Base-925` | `3f2fa7d382419109a7618b50886faae2af748104` | `#111827` | Dark mode card/surface bg |
| `Base/Base-910` | `9a54a05fc4b5fe4286a55987178c6dfe85d43cc7` | `#1A2236` | Dark mode elevated surface |
| `Base/Base-900` | `60221769b400401712fdcd7f87622e026d92e2e8` | `#030D2D` | Primary text, headings |
| `Base/Base-800` | `5b00f6d3ce4bf75bbebbf1739c5de55b42520d0f` | `#1C2542` | Very dark navy |
| `Base/Base-700` | `261c4c6e156b8d81405f13e4f1495460e07ec55d` | `#353D57` | Dark navy-grey |
| `Base/Base-600` | `0a2933abde9dd308b926700b71779276b560e4a0` | `#4F566C` | Secondary text (light mode) |
| `Base/Base-500` | `9def0dd249e14ca795a099b46fca920394664b29` | `#686E81` | Tertiary text, disabled |
| `Base/Base-400` | `188d3920ef1f79870a90e95f50eee3aa917c3b6c` | `#818696` | Secondary icons, light borders |
| `Base/Base-300` | `dc95cee51d9749ee6024ca5a4d2c43c95411c431` | `#9A9EAB` | Placeholder, inactive |
| `Base/Base-200` | `3cd1c141e95f041aabfa6eab5c189d53e8a07d43` | `#B3B6C0` | Pale grey, hover bg |
| `Base/Base-100` | `82f2b0b969ddf49c97ece9663aecd2a4ff76a68b` | `#CDCFD5` | Card borders, dividers |
| `Base/Base-50` | `53dee2fa85c343f2f6a263007c38083b75d62479` | `#E6E7EA` | Tag/chip bg, subtle fills |

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
| `Brand Blue/400 2( Older Hover)` | `c2d6df3b0366538e634bd4e2badb2a7fad6bcacf` | `#3689FF` | Legacy hover blue (deprecated?) |

### Complementary

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Complementary/Pink/500` | `7b8bc797c09ee06fb22849331ba3079351d73a58` | `#C20568` | Hot-pink accent CTAs |
| `Complementary/Pink/400` | `3f21a7ed1998d702d3e85aea6744c81ab9b0d3ad` | `#E31776` | Pink hover |
| `Complementary/Pink/Tint Light` | `0d5c6abce7b5a242e44ea7d72e0521420e23c5f9` | `#C2056812` | Pink hover tint |
| `Complementary/Pink/Tint Dark` | `d3f105bc5eeb046855ccf9ce68ee2c10078effd7` | `#C2056866` | Pink dark bg tint |
| `Complementary/Purple/500` | `f5790114d853bd5bbfa3bde6e9f857fb58633a7e` | `#7B4CFF` | AI features, premium |
| `Complementary/Purple/400` | `848621a0d6399273e37e1acb752908d0c76e121a` | `#9873FF` | Purple hover |
| `Complementary/Purple/Tint Light` | `e9ec26ac53bfb6f6508ee1a40593d374ffb43502` | `#7B4CFF12` | Purple hover tint |
| `Complementary/Purple/Tint Dark` | `8250fbe64d4b363b84a904f0300e200aadd3fbf3` | `#7B4CFF66` | Purple dark bg tint |

### Status

| Token Name | Key | Resolved Value | Usage |
|---|---|---|---|
| `Status/Error` | `38b180f446c75dc88bba0fd75625025271c88cbd` | `#C9392A` | Error red |
| `Status/Error/Dark` | `29c17caca5513ebbc2ce94a111a4529c6787333b` | `#A52E20` | Destructive pressed |
| `Status/Error/Light` | `575e5772c9e0e5f7d4cac3659ed5b807993be5f0` | `#DE5A48` | Error hover on dark |
| `Status/Error/Tint Light` | `f4997f68cff1c4a2a1e06c1b4075c0ca2f13930e` | `#C9392A12` | Error bg fill |
| `Status/Error/Tint Dark` | `4e3def175c4a33d9b81baef97a93420eab15d292` | `#C9392A66` | Error dark bg fill |
| `Status/Warning` | `737cf72094488e099cea340e89fcd68a31ad2999` | `#FFB700` | Warning amber |
| `Status/Warning/Tint Light` | `652e2ee4a18759110fc22145c7f8302204f699f2` | `#FFB70012` | Warning bg fill |
| `Status/Warning/Tint Dark` | `21202:162` | `#FFB70066` | Warning dark bg fill |
| `Status/Success` | `c053dc86923bfc19b7894000e0be6aa9ae6eebcb` | `#16A34A` | Success green |
| `Status/Success/Tint Light` | `1a0263993c3edfaef2ee97e265ad04377bef1fc0` | `#16A34A12` | Success bg fill |
| `Status/Success/Tint Dark` | `21202:164` | `#16A34A66` | Success dark bg fill |
| `Status/Notice` | `a1456e6319fe18823dcff48396098c7047d58170` | `#67C3BB` | Teal — informational |
| `Status/Notice/Tint Light` | `f719b27da1667e4941a384682c9b1d2ad2cf8a97` | `#67C3BB12` | Notice bg fill |
| `Status/Notice/Tint Dark` | `21202:163` | `#67C3BB66` | Notice dark bg fill |

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
| `Background/Container` | `146ff989c79525dc33c46c338611c9f8b40a52f4` | `#FFFFFF` | `#080D1A` |
| `Background/Card On Surface` | `2910233d5d0171d23b8e6f013430570c0bf9896e` | `#FFFFFF` | `#111827` |
| `Background/Card On Container` | (new) | — | — |
| `Background/Surface` | `9cf5e54da014b68dd50661539f573eddd9b359e9` | `#F1F1F1` | `#1A2236` |
| `Background/Surface Lighter` | `c9b03102055b8e5d3498311bba13088a478e89b8` | `#F5F5F5` | `#1A2236` |
| `Background/Surface Darker` | `389caeb17542d338f31bdc962d025d71da5fc3f3` | `#E6E7EA` | `#1C2542` |
| `Background/Element` | (new) | — | — |
| `Background/Element Darker` | (new) | — | — |
| `Background/Element Darkest` | (new) | — | — |
| `Background/Container Darker` | (new) | — | — |
| `Background/Container Darkest` | (new) | — | — |
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
| `Text & Icon/OnColor` | `f9120e3b7cdb03005de1f6c7e665fedb088c42bc` | `#FFFFFF` | `#FFFFFF` |
| `Text & Icon/Brand` | `029b55af59d7b919c8b1d7192bb396793f224dfe` | `#1770EF` | `#1770EF` |

### Border

| Token Name | Key | Light | Dark |
|---|---|---|---|
| `Border/Default` | `80e69d28b62fd63385657c7eaa1f435c2a00e8af` | `#CDCFD5` | `rgba(255,255,255,0.12)` |
| `Border/Hover` | `e99cb844f3ebd39643a10590d0aa2a497d623564` | `#9A9EAB` | `rgba(255,255,255,0.25)` |
| `Border/Focus` | `77eee1910044597fba0971d35cb8db4262b25414` | `#1770EF` | `#4D8FF5` |
| `Border/Error` | `7810d4e2af199f40924a37771f2660644b5c90b1` | `#C9392A` | `#C9392A` |
| `Border/Subtle` | `ec9335d574d992971305e05f5888967b917816ce` | `#E6E7EA` | `rgba(255,255,255,0.12)` |
| `Border/Tint` | `cf5ddadc3f78249005768b63cd32c8a3ea739cef` | `#1770EF24` | `#1770EF24` |
| `Border/Tint Light` | `536500461da06e860eb578270c3d8e497d54362c` | `#1770EF12` | `#1770EF12` |
| `Border/Tint Dark` | `2b2133538868fe0dca3a89528fa6cfe7a85a012a` | `#1770EF66` | `#1770EF66` |
| `Border/Brand Hover` | `b3ec71fd06afde3e0e7086713a71c09950618f14` | `#4D8FF5` | `#4D8FF5` |

### Interactive

| Token Name | Key | Value |
|---|---|---|
| `Interactive/BG/Brand` | `638439cce82a651f0a44efaa97d8e2f4662fce38` | `#1770EF` |
| `Interactive/BG/Brand Tint Hover` | `f4c46365fce817add782eed28fbd39c25af528d1` | `#4D8FF5` |
| `Interactive/BG/Brand Pressed` | `9df5fef7f0a67bb588a87ed3ea69bd138aa8ad40` | `#0D5ED4` |
| `Interactive/BG/Brand Focus Ring` | `2e22d92d1ab36a55696e98830584ba9ef5aeb5e1` | `#1770EF` |
| `Interactive/BG/Hover` | (new) | — |
| `Interactive/BG/Pressed` | (new) | — |
| `Interactive/Border/Brand` | (new) | — |
| `Interactive/Border/Hover` | (new) | — |
| `Interactive/Border/Brand Hover` | (new) | — |
| `Interactive/Border/Brand Pressed` | (new) | — |
| `Interactive/Text & Icon/Hover` | (new) | — |
| `Interactive/Text & Icon/Brand` | (new) | — |
| `Interactive/Text & Icon/Brand Hover` | (new) | — |
| `Interactive/Text & Icon/Brand Pressed` | (new) | — |

### Status (Semantic)

| Token Name | Key | Light | Dark |
|---|---|---|---|
| `Status/Error/Error` | `e7b9e822568c67c08c751d1746f81d881ac4ddd7` | `#C9392A` | `#DE5A48` |
| `Status/Error/Tint` | `193be8a725e3a597c08ada34a4105011f7c7a4a2` | `#C9392A12` | `#C9392A12` |
| `Status/Warning/Warning` | `5e4dea8f7444b1b9cb3df91b44540126c2d3456a` | `#FFB700` | `#FFB700` |
| `Status/Warning/Tint` | `f976093b3fdc0afec0d79037d49a4779c0a69308` | `#FFB70012` | `#FFB70012` |
| `Status/Success/Success` | `72ebda9d531de1aa8bb93d99b03cebccb01231ce` | `#16A34A` | `#16A34A` |
| `Status/Success/Tint` | `e27d2fcfc819b3772c5e9ef6ead235cd021bc88a` | `#16A34A12` | `#16A34A12` |
| `Status/Notice/Notice` | `7225da306e417326845ac2227fb7fd09d7a2d2dd` | `#67C3BB` | `#67C3BB` |
| `Status/Notice/Tint` | `6de68633eba5798b17c1fad24b50df6ce6b747af` | `#67C3BB12` | `#67C3BB12` |
| `Status/Error/Tint Darker` | (new) | — | — |
| `Status/Warning/Tint Dark` | (new) | — | — |

---

## Form Tokens — Collection: .Forms (Light / Dark modes)

> Hidden collection (`.` prefix). Component-scoped tokens for Input and Form components.

| Token Name | Old Name | Type |
|---|---|---|
| `Input/Bg/Default` | `Input Default Bg` | COLOR |
| `Input/Bg/Disabled` | `Input Disabled Bg` | COLOR |
| `Input/Border/Default` | `Input Default Border` | COLOR |
| `Input/Border/Hover` | `Input Hover Border` | COLOR |
| `Input/Border/Focus` | `Input Focus Border` | COLOR |
| `Input/Border/Error` | `Input Error Border` | COLOR |
| `Input/Text/Default` | `Input Default Font Color` | COLOR |
| `Input/Text/Filled` | `Input Filled Font Color` | COLOR |
| `Input/Text/Disabled` | `Input Disabled Font Color` | COLOR |
| `Input/Text/Label` | `Input Label Font Color` | COLOR |
| `Form/Bg/Default` | `Form Bg` | COLOR |

---

## Button Tokens — Collection: .Button Tokens (Light / Dark modes)

> Hidden collection (`.` prefix). Per-button-type color tokens covering 11 button variants.
> Each type provides `Bg/*`, `Text/*`, `Border/*`, and `FocusRing` tokens for all interaction states.

### Primary

| Token Name | States |
|---|---|
| `Primary/Bg/Default` | Default, Hover, Pressed, Disabled, FocusRing |
| `Primary/Text/Default` | Default, Disabled |

### Secondary

| Token Name | States |
|---|---|
| `Secondary/Bg/Default` | Default, Hover, Pressed, Focus, Disabled |
| `Secondary/Text/Default` | Default, Disabled |
| `Secondary/Border/Default` | Default, Hover, Pressed, Disabled |
| `Secondary/FocusRing` | — |

### Tertiary

| Token Name | States |
|---|---|
| `Tertiary/Bg/Hover` | Hover, Pressed, Disabled, FocusRing |
| `Tertiary/Text/Default` | Default, Disabled |
| `Tertiary/Border/Default` | Default, Hover, Pressed, Disabled |

### Danger

| Token Name | States |
|---|---|
| `Danger/Bg/Default` | Default, Hover, Pressed, Focus, Disabled |
| `Danger/Text/Default` | Default, Disabled |
| `Danger/FocusRing` | — |

### Outline

| Token Name | States |
|---|---|
| `Outline/Bg/Hover` | Hover, Pressed |
| `Outline/Text/Default` | Default, Disabled |
| `Outline/Border/Default` | Default, Disabled |
| `Outline/FocusRing` | — |

### OutlineComplementary

| Token Name | States |
|---|---|
| `OutlineComplementary/Bg/Hover` | Hover, Pressed, Focus, Disabled |
| `OutlineComplementary/Text/Default` | Default, Disabled |
| `OutlineComplementary/Border/Default` | Default, Hover, Pressed, Disabled |
| `OutlineComplementary/FocusRing` | — |

### Complementary

| Token Name | States |
|---|---|
| `Complementary/Bg/Default` | Default, Hover |
| `Complementary/Text` | — |

### Link

| Token Name | States |
|---|---|
| `Link/Text/Default` | Default, Hover, Pressed, Focus, Disabled |
| `Link/FocusRing` | — |

### Translucent

| Token Name | States |
|---|---|
| `Translucent/Bg/Default` | Default, Hover, Pressed, Focus, Disabled |
| `Translucent/Text/Default` | Default, Hover, Disabled |
| `Translucent/Border/Default` | Default, Hover, Disabled |
| `Translucent/FocusRing` | — |

### Transparent

| Token Name | States |
|---|---|
| `Transparent/Bg/Hover` | Hover, Pressed, Focus |
| `Transparent/Text/Default` | Default, Disabled |
| `Transparent/FocusRing` | — |

### Blueish

> Note: Blueish uses **paint styles** (not tokens) for Bg states. Only Text, Border, and Disabled Bg are tokenized.

| Token Name | States |
|---|---|
| `Blueish/Text/Default` | Default, Disabled |
| `Blueish/Border/FocusRing` | — |
| `Blueish/Bg/Disabled` | — |

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

## Semantic Spacing Tokens (aliases — resolved from Spacing collection)

### Button Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/button/small/paddingX` | `e26efe371b9d3f2768a1d34060b7975be3660389` | → `s` | `12px` |
| `Semantic/button/small/paddingY` | `ca1d595dab0458a899d5f21e0ca9bd54cc0699d3` | → `xxs` | `4px` |
| `Semantic/button/small/gap` | `59ecbe0a4a861108e35d8fce46e31f565a0362cc` | → `xxs` | `4px` |
| `Semantic/button/medium/paddingX` | `8dd165b387eb863d2799e839ccecb8d6bee92435` | → `m` | `16px` |
| `Semantic/button/medium/paddingY` | `7b32e6df84345d1d10fb392b7bb39c5cd49f997c` | → `xs` | `8px` |
| `Semantic/button/medium/gap` | `ebb76379c70326261fdad217c431f27fa8850ee8` | → `xs` | `8px` |
| `Semantic/button/large/paddingX` | `ff2e8f83bef38c18997fb698ac9ab6ac09becf86` | → `xl` | `24px` |
| `Semantic/button/large/paddingY` | `f08314229169e71269ba7c472a946a2df0550a02` | → `s` | `12px` |
| `Semantic/button/large/gap` | `3113338b166838ddd55db55b730204c0f4cb0dbf` | → `s` | `12px` |
| `Semantic/button/xlarge/paddingX` | `401e4e260a61c1568e2932bd2d8dc9cb147fbf66` | → `xxl` | `32px` |
| `Semantic/button/xlarge/paddingY` | `684ded17c5c520c123c6a4be5c3638be96f7b045` | → `m` | `16px` |
| `Semantic/button/xlarge/gap` | `8458561b4e3208e1f33d178caf06298edc6b098a` | → `s` | `12px` |

### Input Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/input/paddingX` | `5f20c8052de6ab96109c97a5975d4310793a260e` | → `s` | `12px` |
| `Semantic/input/paddingY` | `ed44fc6d3273836c99c10c75aaf2c76eaf33b965` | → `xs` | `8px` |
| `Semantic/input/gap` | `419e5122e159e072e40c180930abc74a9e94d2c2` | → `xs` | `8px` |

### Card Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/card/padding` | `f16fcb85b13ca6a5396bf503be922cf71811c84d` | → `xl` | `24px` |
| `Semantic/card/gap` | `19fc7ceefc6ea4e69eccd0095e4489cab26a282a` | → `m` | `16px` |

### Modal Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/modal/padding` | `2abc296cf4ce8e87ddd32b1becc37d77e0aa4c2f` | → `xl` | `24px` |
| `Semantic/modal/gap` | `4d2d4b3e988bb75cd6ad3f8b17077d0df4697873` | → `l` | `20px` |

### Section Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/section/padding` | `3c7e3142b2d673f8538ce8bc347ef5dd68d0b77f` | → `xxl` | `32px` |
| `Semantic/section/gap` | `b744b2f2f30584448902489b0b2b92fbbad9dfcd` | → `xl` | `24px` |

### Tag Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/tag/paddingX` | `779f4cd504a00272a7640dcf725509018cbb185f` | → `xs` | `8px` |
| `Semantic/tag/paddingY` | `c0177fe6270fc24bff59479002f7f225220f39e4` | → `xxxs` | `2px` |

### Tooltip Spacing

| Token | Key | Alias → | Resolved |
|---|---|---|---|
| `Semantic/tooltip/paddingX` | `37fc0acf2929516bb809dd0f83228cb39fb811bc` | → `xs` | `8px` |
| `Semantic/tooltip/paddingY` | `64dad3a1d08da90fa8e800f3facfe078fa2c7510` | → `xxs` | `4px` |

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
| `Semantic/Container` | `ce0eda81136e73de64572b79314e48d939ada7bd` | `20px` (→ 3xl) |

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
| `size/2xs` | `798691c2357f4c5d4aed8c70439ccc76e6c9e220` | `10px` | `10px` |
| `size/xs` | `2d2ce76c53d63653935f83f89ac9118b92c371b8` | `12px` | `11px` |
| `size/s` | `37a60de618cb2058efa6a0e43377f2bc98cedc91` | `14px` | `13px` |
| `size/m` | `98547d8c5f864ea460160ed3faeaf7002bbbf982` | `16px` | `14px` |
| `size/l` | `aa5debc1bef09591d166a065f3051a9dbccf5bb2` | `20px` | `18px` |
| `size/xl` | `575448093bceb106e21356fe714ef0c7030a9f1e` | `24px` | `20px` |
| `size/2xl` | `74bb7bb9b0d637fc71bb67f8f40a7b072958902b` | `32px` | `28px` |
| `size/3xl` | `abfb7714033539e6bb3cde0fce009fba3c0393e9` | `36px` | `32px` |
| `size/4xl` | `3bab46a795641188ebd84a2c9a4a21f97e1fdb89` | `48px` | `40px` |
| `size/5xl` | `39f02eb04e18f38c3d6585333a2f0fec9c165c70` | `64px` | `56px` |

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

---

## Paint Styles (Color Styles)

### Gradient

| Style Name | Key | Type | Description |
|---|---|---|---|
| `Gradient/Glass` | `4cc34b29c33ec640f15ff85af5f99cd73d4f4837` | Solid #FFFFFF + Linear | White base + linear #0B0223 48%→32% opacity overlay |
| `Gradient/Linear Dark 1` | `7737ba9c51f71ce69f6d24244fb924782faf86a5` | Linear | #000000 4%→64% opacity (top-to-bottom darken) |
| `Gradient/Radial Dark 1` | `05d3711dbfcfac2b781fd7ba0c084fd328fbb466` | Radial | #000000 0%→80% opacity (center-out vignette) |
| `Gradient/Brand Gradient` | `30783afb846c29fb935b0f02fb750d1eae217726` | Radial | #1770EF 14%→7% opacity (subtle brand glow) |
| `Gradient/Blue` | `46d697d0b1f9bca07c29ec50dfab943f5eb57e1d` | Linear | #7B4CFF → #0EA4C5 (purple-to-teal, premium CTA) |
| `Gradient/Blue Hover` | `9159794b64b25132badcda350080ae5ba5f57fc6` | Linear | #9C79FF → #0FD4FF (lighter purple-to-cyan, hover state) |

### BG (Background)

| Style Name | Key | Type | Description |
|---|---|---|---|
| `BG/Inside Page` | `f4b6c3584180aaf72088c7c038dae257f0d39368` | Solid | #F1F1F1 (same as Neutral/Surface) |
| `BG/HomePage BG` | `c33f61eeacb7027624b8bf61a682805ecd5856e5` | Solid + 3 Radials | #F1F1F1 base + purple radial 10% + blue radial 16% + purple radial 10% (ambient brand glow) |

---

## Effect Styles

### Shadows

| Style Name | Key | Type | Color | Offset | Radius | Spread |
|---|---|---|---|---|---|---|
| `Shadow/Small` | `73345d32096a298dcc92258643dc7fbb3b6af800` | Drop | #000000 4% | 0, 2 | 8 | 0 |
| `Shadow/Normal` | `05aff2b3578acdd6dcaa7c9ac5fbdf26f4643be5` | Drop | #000000 8% | 0, 4 | 16 | 0 |
| `Shadow/Big` | `3b10424839bb48fe3900edbb866fa1a834e6ca4b` | Drop | #000000 8% | 0, 8 | 24 | 0 |
| `Shadow / Dark` | `97adb599d587a75c38570826c40a0befb5b80d5d` | Drop | #000000 30% | 0, 4 | 8 | 0 |
| `Shadow/Button Shadow` | `7c6c448dbc2bff72329a68ffb300e37e8c90000e` | Drop | #000000 10% | 0, 8 | 16 | 0 |

### Blurs

| Style Name | Key | Type | Radius |
|---|---|---|---|
| `Blur/Layer Blur - 120` | `3f04553c56503d02b17f1368a6f59f10988c2036` | Layer Blur | 120 |
| `Blur/Bg Blur - Small` | `9758e1dcc36ab48f81d4d41627891bb7f5f8e9bd` | Background Blur | 24 |
| `Blur/Bg Blur - Medium` | `1a58617d36b5524f6238dfae078633f07d7ddd72` | Background Blur | 64 |
| `Blur/Bg Blur - Large` | `059189c60d389e1efb38cd8fab17488aa73f8410` | Background Blur | 120 |

### Border Effects (Inner Shadow)

| Style Name | Key | Direction | Color | Offset |
|---|---|---|---|---|
| `Border/Top` | `55449d0f49c8502fa5dbd655fe7d4301f1511952` | Top | #F5F5F5 100% | 0, 1 |
| `Border/Right` | `f09f7722ec3f26b37a7627866f5a22622ea8e000` | Right | #000000 16% | -1, 0 |
| `Border/Left` | `b97aaf14a8bc895711389bea0732e5eeebdabe14` | Left | #000000 16% | 1, 0 |
| `Border/Bottom` | `4c27b7ef14d37404067ed51369c2157be3c53e3e` | Bottom | #000000 16% | 0, -1 |
