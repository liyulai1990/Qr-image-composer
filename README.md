# 图片二维码合成工具 · Image QR Code Composer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-2.0-blue.svg)](https://github.com/Locallabstide/Qr-image-composer/releases/tag/v2.0)
[![Online Demo](https://img.shields.io/badge/demo-online-brightgreen.svg)](https://Locallabstide.github.io/Qr-image-composer/)

> 纯前端、零依赖、可离线的图片二维码合成工具。把二维码图片批量合成到海报 / 底图上，支持拖拽、缩放、旋转、四边裁剪，一键导出 ZIP。
>
> A pure-frontend, zero-dependency, offline-capable tool to composite QR-code images onto posters / base images. Drag, scale, rotate, crop, and batch-export to ZIP.

🌐 **在线体验 / Live Demo**：https://Locallabstide.github.io/Qr-image-composer/
🔗 仓库地址 / Repo：https://github.com/Locallabstide/Qr-image-composer

![界面预览](screenshot.png)

## ✨ 特性 / Features

- **纯本地**：所有图片在浏览器内处理，不上传任何服务器。 / Fully local — everything runs in your browser, nothing is uploaded.
- **零依赖**：单个 `index.html`，无需联网、无需安装任何库或运行时，双击即用。 / Single `index.html`, no network, no dependencies, no build step.
- **动态 + 固定二维码**：可导入多张动态二维码循环合成，也可固定一张常驻底图。 / Dynamic & fixed QR layers — loop multiple QR images or pin one.
- **精准定位**：X / Y / 缩放 / 旋转 数值微调 + 画布直接拖拽 + 四边裁剪手柄（旋转态用局部坐标系，对边保持固定）。 / Precise positioning with numeric controls and on-canvas handles.
- **批量导出**：按导入顺序批量合成并打包为 ZIP，文件名带时间戳，导出后缀与实际编码格式对齐。 / Batch compose & ZIP export with timestamps.
- **健壮**：底图尺寸 / 像素上限校验、导出期间编辑锁、裁剪边界收敛、拖拽出窗防粘滞、加载竞态令牌。 / Robust guards: size / pixel limits, export lock, drag guards, race-token.

## 🎯 适用场景 / Who is it for?

- 餐饮 / 零售商家制作**带二维码的菜单、海报、传单**（如把点餐 / 外卖 / 会员二维码贴到宣传图上）。
- 运营 / 市场人员批量生成活动二维码图。
- 设计师需要把二维码**精确合成**进设计稿，并保持可重复导出。

## 🚀 快速开始 / Quick Start

1. 打开 [在线体验](https://Locallabstide.github.io/Qr-image-composer/)，或下载 `index.html` 双击运行。
2. 上传底图，再导入一张或多张二维码图片。
3. 通过右侧面板或直接在画布上拖拽、缩放、旋转、裁剪，摆好位置。
4. 点击「批量导出」，生成 `二维码合成结果-YYYYMMDD-HHMMSS.zip`。

更详细的图文说明：

- **[用户操作手册](图片二维码合成工具-用户操作手册.md)** — 面向普通使用者，5 步上手，含导出规则、常见问题与快捷键速查。
- **[开发者手册](图片二维码合成工具-开发者手册.md)** — 面向开发者 / 贡献者，含状态模型、坐标系几何推导、ZIP 编码实现与关键函数索引。

## 🛠 技术说明 / Tech

- 原生 JavaScript + Canvas，无第三方库，无构建步骤。 / Vanilla JS + Canvas, no third-party libs, no build step.
- ZIP 打包为内置的纯 JS 实现（无 JSZip 等外部依赖）。 / ZIP is a built-in pure-JS implementation.
- 完全离线可用，适合分发到不同电脑使用。 / Fully offline — great for distribution across machines.

## 📄 许可 / License

[MIT License](LICENSE) © 2026 Yulai
