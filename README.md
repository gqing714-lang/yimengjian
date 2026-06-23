# 一梦间网页：中文像素字体最终修正

修复了直链字体的 `@font-face` 生成错误：

- 错误：数组使用 `.join('\\n')`，生成的是字面量反斜杠和 n，CSS 无法解析。
- 正确：数组使用 `.join('\n')`，生成正常换行，`@font-face` 可以生效。

默认字体：
- URL：https://cdn.jsdelivr.net/npm/@pixelium/web-vue@0.0.5/dist/fusion-pixel-12px-proportional-zh_hans.ttf.woff2
- 字体名：Fusion Pixel 12px Proportional SC
