# Sketch It

Sketch It is a lightweight web app for turning photos into sketch-like visuals, symbol-based line art, and experimental poster-style renderings.

`Sketch It` 是一个轻量网页工具，可以把照片转换成带有手绘感、符号感、实验海报气质的图像结果。

It is not meant to be a one-click “photo filter”.

它更像是一个可以慢慢调参数、在照片与绘画之间重新寻找视觉语言的小工具。

## Features

- Real-time rendering updates
- Variable line weight with expressive contrast
- Brush / Marker / Sketch line behavior
- Outline emphasis for heavier outer contours and lighter inner structure
- Keep original photo or switch to faded base rendering
- Blur + Frost texture for soft base styling
- Dust / Scratches distress texture
- Braille and Shapes symbol mark modes
- Gems asset brush mode
- Randomized palette-based color rendering
- White-only palette option
- PNG photo export
- SVG export

- 实时更新，不需要反复点击 Render
- 支持更有对比的粗细线条
- 可切换 Brush / Marker / Sketch 三种线条气质
- 可强调外轮廓，让外圈更重、内部更轻
- 可保留原照片，或切换到褪色底图
- 支持 Blur + Frost 底图质感
- 支持 Dust / Scratches 做旧纹理
- 支持 Braille 和 Shapes 符号笔触模式
- 支持 Gems 珠宝 / 宝石组件笔刷模式
- 颜色会基于 palette 随机分配
- 新增纯白 palette
- 可导出 PNG 照片
- 可导出 SVG

## Controls

### Edge

- `Mark style`: choose between normal stroke, braille marks, geometric symbols, or gem assets
- `Threshold`: edge sensitivity
- `Density`: controls how many traced segments remain
- `Stroke min / max`: range of line weight contrast
- `Symbol density`: spacing of symbols along the traced path
- `Size jitter`: random size variation for symbol marks

### Base

- `Ink style`: Sketch / Brush / Marker
- `Outline emphasis`: stronger outer contour, lighter inner detail
- `Keep original photo`: preserve the base image instead of fading it
- `Fade`: how much the photo is washed out
- `Blur`: softness of the base image
- `Frost`: film-grain / noise-like overlay texture
- `Extend`: extends path endings outward
- `Curl`: adds curvature to the path endings

### Texture

- `Dust`: adds subtle dust particles
- `Scratches`: adds distressed scratch marks

## How To Use

1. Upload a photo
2. Adjust edge density and stroke range
3. Choose line behavior with `Ink style`
4. If you want a more experimental result, switch `Mark style` to `Braille` or `Shapes`
5. Use `Keep original photo` on/off depending on whether you want the original image preserved
6. Save the rendered image as PNG or export as SVG

1. 上传图片
2. 调整边缘密度和线条粗细范围
3. 用 `Ink style` 选择线条气质
4. 如果想做更实验的效果，可以把 `Mark style` 切到 `Braille` 或 `Shapes`
5. 根据需求选择是否开启 `Keep original photo`
6. 最后保存 PNG 照片或导出 SVG

## Suggested Combos

### Brush Illustration

- `Mark style`: Stroke
- `Ink style`: Brush
- `Outline emphasis`: 60-80
- `Stroke min`: low
- `Stroke max`: high

### Experimental Poster

- `Mark style`: Shapes
- `Symbol density`: 60-90
- `Size jitter`: 35-70
- high contrast palette

### Gem Brush Drawing

- `Mark style`: Gems
- `Symbol density`: 25-55
- `Size jitter`: 8-22
- white palette or low-saturation palette

### Braille Texture Drawing

- `Mark style`: Braille
- `Symbol density`: 90-120
- `Size jitter`: 10-25
- lower `Stroke min / max` range for a finer result

### Soft Photo + Drawing

- `Keep original photo`: on
- lower `Outline emphasis`
- medium `Density`

## Notes

- `Frost` is currently designed to feel closer to film grain / noise overlay than glass distortion.
- Symbol modes are rendered along traced paths, not randomly scattered over the image.
- Gem mode uses individual SVG assets and now avoids most direct overlaps between pieces.
- SVG export includes line, symbol, and gem-based outputs.

- 目前 `Frost` 更偏向胶片颗粒 / noise overlay 的感觉，而不是玻璃折射。
- 符号模式是沿着路径生成，不是随机铺满整张图。
- Gems 模式使用更大、更稀疏的排布逻辑，并会尽量避开组件之间的直接重叠。
- SVG 导出会保留线条模式、符号模式和 gems 模式的结果。

## Local Usage

This project is a single-file web app.

这个项目目前是单文件网页工具。

You can simply open `index.html` in a browser.

直接在浏览器里打开 [index.html](C:\Users\111\Documents\New project\sketchit-web\index.html) 即可使用。

## License

Personal project by daftlamb.

daftlamb 的个人项目。
