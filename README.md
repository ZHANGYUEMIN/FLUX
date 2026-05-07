# FLUX · 流态人格系统

> 人格不是盒子，而是河流。

[![Deploy](https://github.com/ZHANGYUEMIN/FLUX/actions/workflows/deploy.yml/badge.svg)](https://github.com/ZHANGYUEMIN/FLUX/actions/workflows/deploy.yml)
[![Code: MIT](https://img.shields.io/badge/Code-MIT-c1440e?style=flat-square)](./LICENSE)
[![Content: CC BY-SA 4.0](https://img.shields.io/badge/Content-CC%20BY--SA%204.0-4fc3f7?style=flat-square)](./LICENSE-CONTENT)
[![PWA](https://img.shields.io/badge/PWA-ready-c9a84c?style=flat-square)](./manifest.json)
[![i18n](https://img.shields.io/badge/i18n-zh%20%C2%B7%20en%20%C2%B7%20ja-8a9ba8?style=flat-square)](./index.html)

**在线体验（GitHub Pages）**：[https://zhangyuemin.github.io/FLUX/](https://zhangyuemin.github.io/FLUX/)

**FLUX** 是一套基于动态人格理论的次世代人格框架，比 MBTI 更动态、更连续、更尊重情境。它用三条轴线（SPARK / FRAME / MOVE）刻画你在时间与压力中真实流动的模式。

---

## ✨ 特性

- 🌊 **三轴模型** — 能量来源（SPARK）/ 认知处理（FRAME）/ 行动倾向（MOVE）
- 🎨 **8 种核心流态** — 燃火者 / 领航者 / 引爆者 / 工匠者 / 潜流者 / 织网者 / 解构者 / 深渊者
- 📊 **可视化分数条** — 不只是给你一个标签，更告诉你在每条轴线上的真实位置
- 🪞 **阴影流态分析** — 找到你最不熟悉、却最值得理解的另一面
- 🌐 **多语言** — 简体中文 / English / 日本語，一键切换并记住偏好
- 🔗 **URL 哈希分享** — `#result=RPB` 或 `?lang=en#result=RPB` 可直接打开对应解读
- 📋 **一键复制结果** — 链接 / 文字两种格式
- 🖼️ **保存分享海报** — 结果页导出 PNG（1200×1500），含优势、阴影、成长、领域与品牌水印，便于社交分享
- 📲 **PWA** — `manifest.json` + Service Worker，可「添加到主屏幕」，弱网或离线可打开已缓存页面
- 🌗 **响应式设计** — 桌面 / 平板 / 手机与安全区（刘海屏）适配
- 🐛 **Bug 反馈** — 右下角浮动入口，通过邮件联系作者（预填诊断信息）
- 🚫 **零构建** — 核心为单个 `index.html`；PWA 仅增加静态 `manifest.json` / `sw.js` / `icon.svg`

---

## 🚀 快速开始

### 本地运行

```bash
git clone https://github.com/ZHANGYUEMIN/FLUX.git
cd FLUX

# 建议用本地静态服务器（避免 file:// 下部分 API 受限）
python -m http.server 8080
# 访问 http://localhost:8080
```

或使用 Node：

```bash
npx serve .
```

### 部署到 GitHub Pages

仓库已配置 GitHub Actions（`.github/workflows/deploy.yml`），**推送到 `main` 分支**即自动部署。

1. Fork 或 clone 本仓库  
2. 仓库 **Settings → Pages**  
3. **Build and deployment → Source** 选择 **GitHub Actions**  
4. 等待 workflow 跑完（约 1～2 分钟）

**正式站点**：[https://zhangyuemin.github.io/FLUX/](https://zhangyuemin.github.io/FLUX/)

> 若你 fork 到自己的账号，请将上文链接中的用户名与仓库名替换为你的 `https://<用户名>.github.io/<仓库名>/`。

---

## 🧭 三条轴线

| 轴    | 代号        | 极点          | 含义               |
| ---- | --------- | ----------- | ---------------- |
| 能量来源 | **SPARK** | R 辐射 ↔ A 吸收 | 你的精力如何充电、如何消耗？   |
| 认知处理 | **FRAME** | P 模式 ↔ D 细节 | 你的大脑优先处理什么？      |
| 行动倾向 | **MOVE**  | B 突破 ↔ S 稳固 | 面对未知，你倾向于冲破还是守护？ |

---

## 🌊 八种核心流态

| 代码    | 名称  | 一句话         |
| ----- | --- | ----------- |
| `RPB` | 燃火者 | 点燃房间，也点燃自己  |
| `RPS` | 领航者 | 掌舵，但从不离船    |
| `RDB` | 引爆者 | 用数据点燃革命     |
| `RDS` | 工匠者 | 把细节做到极致     |
| `APB` | 潜流者 | 安静地颠覆       |
| `APS` | 织网者 | 在沉默中理解整个系统  |
| `ADB` | 解构者 | 把每件事拆开重组    |
| `ADS` | 深渊者 | 安静地，比任何人都深入 |

每个类型的解读包含：核心描述、优势、阴影面、适配领域、成长建议、阴影流态镜像。

---

## 🛠 技术栈

- **0 框架**：纯 HTML / CSS / 原生 JavaScript  
- **0 构建**：无需 webpack / vite / `npm install`（可选仅用于本地预览工具）  
- **0 后端**：测验、结果、海报生成均在浏览器内完成  
- **字体**：Google Fonts（Noto Serif SC / Noto Serif JP / Space Mono / Raleway）  
- **图标**：内联 SVG favicon + 仓库内 `icon.svg`（PWA）

---

## 📁 目录结构

```
FLUX/
├── index.html              # 主页面（样式、逻辑、多语言字典）
├── manifest.json           # PWA 清单
├── sw.js                   # Service Worker（离线壳）
├── icon.svg                # PWA / 安装图标
├── README.md
├── LICENSE                 # MIT（源代码）
├── LICENSE-CONTENT         # CC BY-SA 4.0（框架与文案内容）
├── .gitignore
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages 部署
```

---

## 🔖 版本与回滚

- 稳定基线可使用 Git 标签 **`v1.0`**（海报与 PWA 之前的首发形态）。  
- 日常开发在 `main`；如需对比历史功能，可 `git checkout v1.0` 本地查看。

---

## 🤝 贡献

欢迎 PR：

- 修复文案 / 翻译  
- 增加题目或调整计分逻辑  
- 加入新语言  
- 优化可访问性（a11y）与海报排版  
- 修 bug  

提交前请尽量保持改动清晰可审；若拆分 `index.html`，请在 PR 中说明理由。

---

## 📜 许可证 · 双许可（Dual License）

本项目采用双许可模式，分别覆盖「代码」与「内容」：

### 💻 代码部分 — [MIT](./LICENSE)

- HTML、CSS、JavaScript、GitHub Actions 等技术与配置  

### 🎨 内容部分 — [CC BY-SA 4.0](./LICENSE-CONTENT)

- FLUX 三轴六极、八种流态命名与全部描述、题目与解读文案  

**推荐署名示例**：

> FLUX 流态人格系统 — © HAPPY Games，内容以 CC BY-SA 4.0 授权  
> [https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

---

**Copyright © 2026 HAPPY Games. All Rights Reserved.**  
**仓库**：[github.com/ZHANGYUEMIN/FLUX](https://github.com/ZHANGYUEMIN/FLUX)

---

## 📮 联系作者 / Contact

- **网站内反馈**：右下角浮动按钮（通过本地邮件客户端发送，预填环境与 URL）  
- **邮箱**：[happy_games@vip.qq.com](mailto:happy_games@vip.qq.com)  
- **GitHub Issues**：[ZHANGYUEMIN/FLUX/issues](https://github.com/ZHANGYUEMIN/FLUX/issues)

人格是河流，不是容器。
