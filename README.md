# qzezhou.github.io — 个人主页

纯静态单文件页面，无外部依赖、无构建步骤、无网络字体请求，离线也能完整显示。

## 本地预览

任选一种即可：

1. **直接双击打开**
   双击 `index.html`，浏览器就能打开。鼠标移动时会有跟随聚光，向下滚动时各区块淡入。

2. **本地服务器（可选，更接近线上效果）**
   ```bash
   cd qzezhou.github.io
   python -m http.server 8000
   ```
   然后访问 http://localhost:8000

## 文件说明

| 文件 | 作用 |
| --- | --- |
| `index.html` | 全部内容：HTML 结构、内联 CSS、内联 JS（齿轮生成、聚光、滚动淡入） |
| `README.md` | 本说明 |

没有 `package.json` / 锁文件，因为项目不使用任何依赖或构建工具。

## 设计说明

整体是机械制图的蓝图风格：深色坐标网格、FIG. 编号、规格表、十字标注、缓慢旋转的齿轮。
配色只用墨蓝底 + 冷蓝线条 + 一点暖黄作高亮。

## 修改内容

所有文字都在 `index.html` 里，直接搜索中文即可定位；主题色在 `<style>` 顶部的 `:root` 变量里改。

## 部署

仓库名为 `qzezhou.github.io` 且为公开仓库，`index.html` 位于仓库根目录，推送后 GitHub Pages 会自动发布到
https://qzezhou.github.io/
