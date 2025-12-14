# Open-Source-AI-drawing-board-Experimental---ai-
An open-source AI canvas built to lower the barrier for AI art education. Developed through a multi-day collaborative process with AI, where I architected the logic to solve API fragmentation and the AI assisted in implementation. It runs purely in the browser, offering a cost-effective alternative for beginners.
# Open Source AI Drawing Board (Experimental)

[English](README.md) | 

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-0.37-green.svg)
![Vue.js](https://img.shields.io/badge/Made%20with-Vue.js-42b883.svg)

> An open-source, node-based AI canvas running entirely in the browser.

## 📖 Introduction

This project is a visual interface for Generative AI. It allows users to drag and drop nodes to construct image generation workflows flexibly.

Designed as a **Client-Side (Pure Frontend)** application, it connects directly to AI APIs (OpenAI/Gemini) from your browser. This eliminates the need for high-end hardware or complex backend installations, making it an accessible tool for learning and experimentation.

## 💡 Why I Built This? (The Story)

I have been involved in **AI Art Popularization and Education**. During this process, I identified two major barriers for beginners and teachers:
1.  **High Costs**: Many platforms require monthly subscriptions, making it difficult to share workflows or for students to practice freely.
2.  **Hardware Limits**: Local tools (like ComfyUI) often require powerful GPUs, which not everyone possesses.

I wanted to create a solution that lowers these barriers.
*   **For Beginners**: A tool that runs on most computers with a browser, sufficient for learning the logic of AI workflows.
*   **The Goal**: To solve the **API Fragmentation** problem (unifying OpenAI and Google Gemini protocols) so users can focus on creativity rather than technical configurations.

## 🤝 Development Journey: Human-AI Collaboration

I want to be transparent: **This project was built through a collaboration between a Human Product Manager and AI.**

This process represents a multi-day journey of iterative product development:
*   **My Role (Product Manager & Creator)**: I identified the user needs in AI education, conceptualized the product features, and defined the logic to handle complex API behaviors (such as Gemini's protocol shifts). I directed the development strategy and verified the results.
*   **AI's Role (Developer)**: Under my guidance, the AI assisted in writing the code, implementing the UI logic, and iterating on specific functions to meet the product requirements.

We solved problems step-by-step—from basic node rendering to complex data handling. This project stands as a sincere experiment in how **Product Thinking** can leverage AI to build real software.

## ✨ Key Features

*   **Adaptive Parser**: Automatically handles various API response formats (Base64, JSON, URLs) from different providers and proxies.
*   **Smart Routing**: Intelligently switches protocols between OpenAI and Google Gemini based on your model selection.
*   **Local Gallery (IndexedDB)**: Saves your generated images persistently in the browser database, solving the issue of data loss upon refresh.
*   **Low Barrier to Entry**: No backend server required. Your API keys and data never leave your device.

## 🚀 Quick Start

No installation needed. No Node.js required.

1.  **Download**: Clone this repo or download the `index.html` file.
2.  **Open**: Double-click `index.html` to open it in Chrome, Edge, or Firefox.
3.  **Setup**:
    *   Click **Settings** (top right).
    *   Add your API Key (OpenAI or Gemini).
    *   Start creating!

## 🛠️ Tech Stack

*   **Framework**: Vue.js 3 (Composition API)
*   **Styling**: Tailwind CSS
*   **Data Storage**: IndexedDB (via idb-keyval)
*   **Tools**: JSZip (for downloading images)

## 📄 License

This project is licensed under the **MIT License**.

---
*Created by Junjun Huai- 2025*


# Open Source AI Drawing Board (Experimental)

 [中文](README_zh.md)

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-0.37-green.svg)
![Vue.js](https://img.shields.io/badge/Made%20with-Vue.js-42b883.svg)

> 一个基于浏览器原生的、开源节点式 AI 画布。

## 📖 项目简介

这是一个可视化的 AI 工作流编辑工具。它允许用户通过拖拽和连接“节点”来构建生图流程。

作为一款 **纯前端（Client-Side）** 应用，它不需要复杂的后台部署，也不需要昂贵的显卡，直接通过浏览器调用 AI 接口即可运行。

## 💡 开发故事与初衷

在从事 **AI 绘画科普** 的过程中，我发现初学者和老师们面临着很高的门槛：
1.  **成本高**：主流生图平台通常需要开通会员，不方便分享，学生的试错成本也很高。
2.  **配置难**：本地部署的专业工具（如 ComfyUI）对电脑硬件配置要求极高，劝退了很多人。

因此，我想做一个 **低门槛** 的 AI 画布。它可能并不完美，但对于初学者理解 AI 工作流逻辑来说已经足够了。

为了实现这个目标，我定义了产品的核心逻辑，旨在解决各大厂商 **API 协议不统一** 的问题，让用户只需关注创作，减少对底层技术的困扰。

## 🤝 开发之旅：人与 AI 的协作

我想真诚地说明：**本项目是在 AI 的辅助下完成开发的。**

但这绝不是“一键生成”的产物，而是一个**历经多天、不断迭代**的产品落地过程：
*   **我的角色（产品经理/发起人）**：我负责挖掘教育场景下的痛点，将抽象的需求具象化为产品功能。我设计了解决 API 兼容性的逻辑方案（例如如何处理 Gemini 的协议变更），并主导了产品的测试与迭代方向。
*   **AI 的角色（开发执行）**：在我的指导下，AI 辅助完成了代码的编写与重构，将产品构想转化为实际运行的程序。

这是一个将 **“产品思维”** 与 **“AI 编程能力”** 结合的实践，展示了非传统程序员如何利用 AI 工具解决实际问题。

## ✨ 核心功能

*   **自适应解析器**：能够识别并处理 API 返回的多种格式（如图片链接、Base64 编码或嵌套 JSON），无需用户手动配置。
*   **智能协议路由**：系统会自动判断你连接的是 OpenAI 还是 Google Gemini，并发送适配的请求格式。
*   **本地图库 (IndexedDB)**：利用浏览器数据库技术，实现了海量图片的本地持久化存储，解决了网页刷新数据丢失的问题。
*   **低门槛使用**：无需安装 Python 或 Node.js，下载一个 HTML 文件即可运行，保护用户隐私。

## 🚀 快速开始

下载即用，无需配置环境。

1.  **下载**：下载本项目中的 `index.html` 文件。
2.  **运行**：直接使用 Chrome、Edge 或 Firefox 浏览器打开该文件。
3.  **配置**：
    *   点击右上角的 **设置**。
    *   输入你的 API Key (支持 OpenAI 或 Gemini)。
    *   开始拖拽节点进行创作！

## 🛠️ 技术栈

*   **核心框架**: Vue.js 3
*   **界面样式**: Tailwind CSS
*   **数据存储**: IndexedDB (idb-keyval)
*   **文件处理**: JSZip

## 📄 许可协议

本项目遵循 **MIT License** 开源协议。

---
*Created by Junjun Huai - 2025*
