# 🎨 Chat with GeoGebra

一个基于自然语言的智能 GeoGebra 几何绘图助手。

通过与大语言模型（LLM）对话，用自然语言描述几何问题，自动生成 GeoGebra 命令并实时绘图。

## ✨ 功能特色

- 🧠 **自然语言交互** - 用中文或英文描述几何问题，AI 自动生成绘图命令
- 🖼️ **实时绘图** - 基于 GeoGebra 强大的几何引擎，即时可视化
- 🔗 **多模型支持** - 支持 OpenAI、DeepSeek、Google Gemini、Anthropic Claude、Azure OpenAI 及自定义端点
- 🌐 **轻量网页版** - 无需安装，浏览器直接访问
- 🔑 **隐私安全** - API Key 仅存储在本地浏览器

## 🚀 快速开始

### 1. 安装依赖

```bash
cd chat-geogebra-intermediate
npm install
```

### 2. 启动服务

```bash
npm start
```

访问 http://localhost:3000

### 3. 配置 API Key

点击右上角"设置"，选择模型提供商并填入 API Key。

支持的提供商：
- OpenAI (GPT-4o, GPT-4o-mini, o1...)
- DeepSeek (deepseek-chat, deepseek-coder...)
- Google Gemini (gemini-2.0-flash, gemini-2.5-pro...)
- Anthropic Claude (claude-3-5-sonnet, claude-3-opus...)
- Azure OpenAI
- OpenAI 兼容端点

## 📝 使用示例

**输入：**
> 画一个边长为 5 的正方形，并画出它的内切圆

**AI 响应：**
生成 GeoGebra 命令并自动执行：
```geogebra
A = (0, 0)
B = (5, 0)
C = (5, 5)
D = (0, 5)
poly1 = Polygon(A, B, C, D)
O = Center(poly1)
circle1 = Circle(O, 2.5)
```

## 🛠️ 技术栈

- **前端**：原生 HTML/CSS/JavaScript
- **后端**：Node.js + Express
- **AI SDK**：Vercel AI SDK
- **几何引擎**：GeoGebra Web API

## 📁 项目结构

```
chat-geogebra-intermediate/
├── server.js          # Express 后端服务
├── package.json       # 项目配置
├── public/
│   └── index.html     # 前端界面
└── README.md          # 项目说明
```

## 🔧 开发模式

```bash
# 监视模式（自动重启）
npm run dev
```

## 📜 开源协议

MIT License

## 👤 作者

Ivory (https://github.com/alexaisophie)

---

*让几何绘图像说话一样简单* 🎯
