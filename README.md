# 云枢产品矩阵官网

云枢（Yunshu Suite）产品矩阵的静态展示站点，介绍从数据治理、智能体执行到 Agent 运营的三层产品体系。

**在线仓库：** [github.com/RandyChen1985/yunshu-website](https://github.com/RandyChen1985/yunshu-website)

## 产品矩阵

| 产品 | 说明 | 仓库 |
|------|------|------|
| 云枢 · 数据服务平台 | 企业级 Data API 与元数据治理，将物理表、SQL 与语义元数据封装为可审计、可授权的 RESTful API | [yunshu-api-data-platform](https://github.com/RandyChen1985/yunshu-api-data-platform) |
| 云枢 · 智能体平台 | AI 智能中枢，涵盖多专家路由、ChatBI、知识库、MCP 工具与嵌入式 Chat SDK | [yunshu-ai-agent-platform](https://github.com/RandyChen1985/yunshu-ai-agent-platform) |
| OpenClaw Buddy | OpenClaw 的 Web 管理台与对话伴侣，可视化配置 Bot、模型、渠道与 Workspace | [openclaw-buddy](https://github.com/RandyChen1985/openclaw-buddy) |

## 技术栈

纯静态站点，无构建步骤、无第三方框架依赖：

- HTML5 + 语义化结构
- 原生 CSS（CSS 变量、Grid / Flexbox 布局）
- 原生 JavaScript（导航滚动、移动端菜单）

## 项目结构

```
.
├── index.html          # 主页面
├── styles.css          # 全局样式
├── script.js           # 交互逻辑（顶栏滚动、移动导航）
├── assets/
│   ├── favicon.svg
│   └── images/         # 产品截图与展示图
└── .gitignore
```

## 本地预览

任意静态文件服务器均可，例如：

```bash
# Python 3
python3 -m http.server 8080

# 或使用 npx
npx serve .
```

浏览器访问 `http://localhost:8080` 即可。

也可直接用浏览器打开 `index.html` 查看，但建议使用本地服务器以避免部分资源加载限制。

## 部署

将仓库内容上传至任意静态托管服务即可，例如：

- GitHub Pages
- Nginx / Caddy 静态目录
- 对象存储 + CDN（OSS、S3 等）

无需编译或环境变量配置。

## 页面结构

- **Hero** — 产品矩阵总览与核心定位
- **产品** — 三层产品介绍与 GitHub 链接
- **架构** — 数据源 → 数据服务化 → 智能体执行 → 运营渠道
- **场景** — ChatBI、数据产品发布、RAG、MCP、SDK 嵌入、Agent 运营
- **交付** — 私有化部署、安全权限、可观测性
- **联系** — 邮件与微信公众号

## 联系

- 邮箱：[cexlong@gmail.com](mailto:cexlong@gmail.com)

---

Connect Data. Orchestrate Intelligence. Operate Agents.
