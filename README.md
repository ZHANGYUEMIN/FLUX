# FLUX · 流态人格系统

> 人格不是盒子，而是河流。

[Deploy](https://github.com/YOUR_USERNAME/flux/actions/workflows/deploy.yml)
[Code: MIT](./LICENSE)
[Content: CC BY-SA 4.0](./LICENSE-CONTENT)
[Pages](https://YOUR_USERNAME.github.io/flux/)

**FLUX** 是一套基于动态人格理论的次世代人格框架，比 MBTI 更动态、更连续、更尊重情境。它用三条轴线（SPARK / FRAME / MOVE）刻画你在时间与压力中真实流动的模式。

🌐 **在线体验**: [https://YOUR_USERNAME.github.io/flux/](https://YOUR_USERNAME.github.io/flux/)

---

## ✨ 特性

- 🌊 **三轴模型** — 能量来源（SPARK）/ 认知处理（FRAME）/ 行动倾向（MOVE）
- 🎨 **8 种核心流态** — 燃火者 / 领航者 / 引爆者 / 工匠者 / 潜流者 / 织网者 / 解构者 / 深渊者
- 📊 **可视化分数条** — 不只是给你一个标签，更告诉你在每条轴线上的真实位置
- 🪞 **阴影流态分析** — 找到你最不熟悉、却最值得理解的另一面
- 🔗 **URL 哈希分享** — `#result=RPB` 可直接打开任意类型的解读
- 📋 **一键复制结果** — 链接 / 文字两种格式
- 🌗 **响应式设计** — 桌面 / 平板 / 手机适配
- 🚫 **零依赖** — 单个 HTML 文件，无构建，无后端

---

## 🚀 快速开始

### 本地运行

```bash
git clone https://github.com/YOUR_USERNAME/flux.git
cd flux

# 直接用浏览器打开 index.html，或者起一个最简单的本地服务器：
python -m http.server 8080
# 然后访问 http://localhost:8080
```

或者，如果你装了 Node：

```bash
npx serve .
```

### 部署到 GitHub Pages

仓库内置 GitHub Actions 工作流（`.github/workflows/deploy.yml`），推到 `main` 分支即自动部署。

1. Fork 或 clone 本仓库
2. 进入 **Settings → Pages**
3. **Source** 选择 `GitHub Actions`
4. push 一次代码即可触发部署

部署后访问：`https://<你的用户名>.github.io/<仓库名>/`

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
- **0 构建**：无需 webpack / vite / npm install
- **0 后端**：所有逻辑在浏览器里完成
- **字体**：Google Fonts（Noto Serif SC / Space Mono / Raleway）
- **图标**：内联 SVG，含 SVG favicon（无外部资源）

整个项目就是 **一个 `index.html`**——可以放进任何静态托管：GitHub Pages、Vercel、Netlify、Cloudflare Pages、自己的 Nginx 都行。

---

## 📁 目录结构

```
flux/
├── index.html              # 主页面（含全部样式与逻辑）
├── README.md               # 你正在读的这个
├── LICENSE                 # MIT 协议（代码部分）
├── LICENSE-CONTENT         # CC BY-SA 4.0（人格框架内容部分）
├── .gitignore
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages 自动部署
```

---

## 🤝 贡献

欢迎 PR：

- 修复文案 / 翻译
- 增加题目或调整计分逻辑
- 加入新语言（English、日本語…）
- 优化可访问性（a11y）
- 修 bug

提交前请保持单文件结构（除非有非常充分的理由拆分）。

---

## 📜 许可证 · 双许可（Dual License）

本项目采用双许可模式，分别覆盖"代码"与"内容"两个层面：

### 💻 代码部分 — [MIT](./LICENSE)

- HTML 结构、CSS 样式、JavaScript 逻辑
- GitHub Actions 工作流、构建配置
- 任何技术性资产

你可以自由地复制、修改、商用、闭源衍生，**只需保留 `HAPPY Games` 的版权声明**。

### 🎨 内容部分 — [CC BY-SA 4.0](./LICENSE-CONTENT)

- FLUX 人格框架的设计（三轴 SPARK / FRAME / MOVE，6 个极点）
- 8 种核心流态命名（燃火者 / 领航者 / 引爆者 / 工匠者 / 潜流者 / 织网者 / 解构者 / 深渊者）
- 全部类型描述、优势/阴影、成长建议、Tagline、9 道题目文案

你可以自由分享、改编、商用，但必须满足两条：

1. **署名** — 必须标注 "© HAPPY Games"，并附上协议链接
2. **相同方式共享** — 你的衍生内容也必须采用 CC BY-SA 4.0 协议

### 📌 推荐署名格式

> FLUX 流态人格系统 — © HAPPY Games，CC BY-SA 4.0 协议授权
> [https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

---

**Copyright © 2026 [HAPPY Games](https://github.com/YOUR_USERNAME). All Rights Reserved.**

---

## 📮 联系作者 / Contact

- **Bug 反馈 / Bug Report**：网站右下角的浮动按钮一键发送（含诊断信息）
- **邮箱 / Email**：[happy_games@vip.qq.com](mailto:happy_games@vip.qq.com)
- **GitHub Issues**：欢迎在仓库中提 Issue 或 Pull Request

人格是河流，不是容器。