# 晓风残月 · 欢迎页 v8 — 柳叶纷飞

## 变更摘要
按用户要求：删除芦草、重新加入柳叶飘落系统并放大柳叶尺寸。

## 关键变更
1. **删除芦草**：移除左右两侧的 SVG 芦草（reeds-left / reeds-right），包括 CSS 样式、`@keyframes reedSway` 动画、HTML 元素、reduced-motion 和响应式引用
2. **恢复柳叶飘落**：重新加入 `.willow-leaf-fall` 容器、`.willow-leaf` 样式、`@keyframes leafFall` 动画、`initWillowLeaves()` JS 生成函数
3. **柳叶放大**：
   - 叶宽：原 10-24px → 22-50px（`w = 22 + Math.random() * 28`）
   - 叶高：`w * 2.5` 等比放大
   - SVG 内部：椭圆 rx 4→5, ry 20→22；中脉 opacity 0.4→0.45
   - 飘落水平摆动幅度加大（translateX 15→25px, -10→-18px 等）
4. **版本标识**：v7→v8，副标题"晓风拂岸"→"柳叶纷飞·晓风拂岸"

## 保留元素
- 巨月 + 三层月晕 + 月尖微星
- 星空 Canvas
- 晨光射线
- 流云
- 晨雾
- 飞鸟
- 水面（surface + shimmer + ripple + sparkles）
- 水中月影（主 + 碎片）
- 地平线晚霞光带
- 标题 / 进入按钮 / 鼠标视差

## 删除内容（累积）
- v5: 远山三层 SVG + 渔舟 SVG
- v6: 右侧垂柳 SVG + 柳幔华盖 SVG
- v7: 水墨柳树图片 + 柳叶飘落系统
- v8: 左右芦草 SVG

## 文件
- `site/index.html` — 所有修改集中于此
