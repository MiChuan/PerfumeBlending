<div align="center">

# 香境 · PerfumeBlending

**一炷烟中得意，九衢尘里偷闲。**

撷取《香乘》等古籍香方之雅 · 融现代香水前中后调之趣 · 纯原生前端实现

[![GitHub Pages](https://img.shields.io/github/deployments/MiChuan/PerfumeBlending/github-pages?label=GitHub%20Pages&logo=github)](https://michuan.github.io/PerfumeBlending/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-CSS3%20%2F%20JS-orange?logo=html5)](index.html)
[![零依赖](https://img.shields.io/badge/dependencies-0-blueviolet)](index.html)

[在线体验](https://michuan.github.io/PerfumeBlending/) · [报告问题](https://github.com/MiChuan/PerfumeBlending/issues) · [香方目录](PerfumeFormula/)

</div>

---

## 关于本项目

一个中国风调香主题网站。收录七方合香——既有《香乘》体系的古法香方（沧澜撷芳、鹅梨帐中香、四合香、十三香），亦有融合现代香水「前调 / 中调 / 后调」结构的创新之作（山茶桃烬、木骨澂澜、泠海芳沉）。

网站以纯原生 HTML / CSS / JavaScript 构建，**单文件、零依赖、零构建**，并内置一款模拟和香的互动小游戏，让访客亲手调配一炉属于自己的香。

## ✨ 功能特性

| 模块 | 说明 |
| ---- | ---- |
| 🎨 **水墨动效背景** | 墨晕云层缓慢漂移 + 飘落香料粒子，宣纸 / 朱砂 / 琥珀金 / 青玉配色 |
| 📜 **香方雅集** | 七方合香卡片，含香铭、故事、香料配比条形图（滚动触发动画） |
| ⚗️ **制香手法** | 选材配伍 → 炮制修治 → 捣碾成粉 → 和泥成型 → 窖藏陈化，五步详解 |
| 🏮 **非遗技艺** | 药香同源、窖藏陈化、打香篆、香席雅集四大板块 |
| 🎮 **模拟和香** | 拖动香料按「君臣佐使」配伍，系统实时打分并给出改进建议 |

## 🚀 快速开始

### 本地运行

```bash
# 1. 克隆仓库
git clone https://github.com/MiChuan/PerfumeBlending.git
cd PerfumeBlending

# 2. 任选一种方式启动
python -m http.server 8000      # Python
npx serve .                     # Node.js

# 3. 浏览器访问 http://localhost:8000
```

也支持直接用浏览器双击打开 `index.html` —— 项目没有任何构建步骤。

## 🌐 GitHub Pages 部署

仓库根目录已有 `index.html`，因此**无需任何构建流水线**，一次配置即可上线：

1. 打开仓库 → **Settings**（设置）→ 左侧 **Pages**；
2. **Build and deployment** → **Source** 选择 **`Deploy from a branch`**；
3. **Branch** 选择 **`main`**，目录选择 **`/ (root)`**，点击 **Save**；
4. 等待约 1–2 分钟，于 `https://michuan.github.io/PerfumeBlending/` 访问即可。

> **提示**：后续每次向 `main` 推送代码，GitHub Pages 都会自动重新构建发布，无需额外操作。

## 📁 项目结构

```
PerfumeBlending/
├── index.html                # 网站主文件（含全部样式与交互逻辑）
├── PerfumeFormula/           # 香方数据源
│   ├── 十三香.md
│   ├── 四合香.md
│   ├── 山茶桃烬.md
│   ├── 木骨澂澜.md
│   ├── 沧澜撷芳.md
│   ├── 泠海芳沉.md
│   └── 鹅梨帐中香.md
├── LICENSE                   # MIT 开源协议
└── README.md
```

## 🛠 技术栈

- **HTML5** — 语义化结构
- **CSS3** — 原生动画、渐变、滤镜，无预处理器
- **原生 JavaScript (ES6+)** — 无框架、无第三方库
- **字体** — [Noto Serif SC](https://fonts.google.com/)（正文）& [Ma Shan Zheng](https://fonts.google.com/)（标题）

浏览器要求：支持现代 CSS 与 ES6 的任意主流浏览器（Chrome / Edge / Firefox / Safari）。

## 📜 香方一览

| 香方 | 类型 | 特色 |
| :--- | :--- | :--- |
| **沧澜撷芳** | 古法合香 | 芽庄沉香为骨，鹅梨为瓮蒸溜三遍，阴干窖藏六十日 |
| **鹅梨帐中香** | 宋人帐中香 | 降真香、檀香、沉香配槐花蜜，凿空鹅梨为香 |
| **十三香** | 药香 · 辛香 | 花椒、干姜、肉桂等十三味本草，温中理气 |
| **山茶桃烬** | 现代香调 | 莓果桃杏 → 玫瑰紫罗兰山茶 → 麝香龙涎檀木 |
| **木骨澂澜** | 现代香调 | 苹果甜橙柚子 → 海洋铃兰茉莉 → 木香收束 |
| **四合香** | 古法简易合香 | 荔枝壳、陈皮、香梨、柏树子四味相合 |
| **泠海芳沉** | 现代香调 | 柑橘粉胡椒海洋 → 玫瑰牡丹莲花 → 雪松龙涎麝香 |

## 🎮 模拟和香玩法

1. 系统随机生成一炉「目标香方」，标注君臣佐使的目标配比；
2. 拖动滑杆，投入沉香、檀香、雪松、玫瑰、龙涎等七种香料；
3. 点击「焚香成韵」，系统按配比契合度评出 **炉火纯青 / 渐入佳境 / 差之毫厘** 三档；
4. 结果面板会指出多放、少放了哪些香料，可「重开一炉」反复挑战。

<details>
<summary><b>计分规则</b></summary>

满分为 100 分，依次扣除：

- 投入目标之外的香料：每 1% 扣 1.4 分
- 遗漏目标中的香料：每 1% 扣 0.9 分
- 目标香料的配比偏差：每 1% 扣 0.8 分

≥ 85 分为炉火纯青，≥ 60 分为渐入佳境，其余为差之毫厘。

</details>

## 🤝 贡献指南

欢迎提交 Issue 与 Pull Request！

- **新增香方**：在 `PerfumeFormula/` 下按既有格式新建 `.md`，并在 `index.html` 的 `recipes` 数组中追加条目；
- **修正错漏**：古籍香方考据、配比勘误尤其欢迎；
- **改进体验**：动效、无障碍、移动端适配等。

提交 PR 前请确保页面在本地可正常渲染，且未引入外部依赖。

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源，可自由使用、修改与分发。

<div align="center">

**谨以香火，敬承古法。**

</div>
