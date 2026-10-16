# 第三方资源与导出包装说明

本仓库的 MIT 许可证适用于项目原创代码和文档，不改变第三方组件或保留的导出运行时包装的权利归属。

## 运行时脚本引用

`dist/index.html` 内“曲率与幅度”组件的导出包装引用以下固定版本脚本。它们通过 UNPKG 在浏览器中加载，第三方库文件未复制进本仓库。

| 组件 | 固定版本 | 上游许可证及归属 | 加载地址 |
| --- | --- | --- | --- |
| `@floating-ui/core` | 1.7.3 | MIT；Floating UI contributors | <https://unpkg.com/@floating-ui/core@1.7.3/dist/floating-ui.core.umd.min.js> |
| `@floating-ui/dom` | 1.7.4 | MIT；Floating UI contributors | <https://unpkg.com/@floating-ui/dom@1.7.4/dist/floating-ui.dom.umd.min.js> |
| `lucide` | 1.17.0 | ISC；Lucide Icons and Contributors；部分 Feather 衍生图标另保留 MIT 归属 | <https://unpkg.com/lucide@1.17.0/dist/umd/lucide.js> |

许可证与来源：

- Floating UI：[源码仓库](https://github.com/floating-ui/floating-ui)、[core 1.7.3 LICENSE](https://unpkg.com/@floating-ui/core@1.7.3/LICENSE)、[dom 1.7.4 LICENSE](https://unpkg.com/@floating-ui/dom@1.7.4/LICENSE)。已核对两个包的固定版本元数据为 MIT；core 1.7.3 的许可证版权行为 `Copyright (c) 2021-present Floating UI contributors`。
- Lucide：[源码仓库](https://github.com/lucide-icons/lucide)、[上游 LICENSE](https://github.com/lucide-icons/lucide/blob/main/LICENSE)、[1.17.0 LICENSE 地址](https://unpkg.com/lucide@1.17.0/LICENSE)。已读取的上游 LICENSE 为 ISC，包含 `Copyright (c) 2026 Lucide Icons and Contributors`，并列明 Feather 衍生图标的 MIT 许可及 `Copyright (c) 2013-present Cole Bemis`。固定版本 LICENSE 的在线获取在本次整理时超时，因此不声称已逐字核对该版本许可文本。

如果将上述库下载并随项目重新分发，请同时保留相应版本的完整许可证、版权声明及上游归属说明。仅存在于 CSP 允许列表的其他域名不代表项目实际加载了对应依赖。

## 原始可视化导出包装

“曲率与幅度”组件来自项目现有的 Codex 可视化 HTML 导出文件。本次开源保留其 iframe、`srcdoc` 内容、CSP、消息通信及本地状态逻辑；不将导出运行时包装声明为项目原创，也不通过项目 MIT 许可证重新授予第三方权利。

包装读取的是访问者自己浏览器中的组件状态，本仓库不包含导出时保存的个人状态数据。源码中出现的 OpenAI 相关标识或图标注释不代表本项目获得 OpenAI 官方背书。

## 独立 Cobb 组件与截图

`dist/cobb.html` 使用原生 JavaScript 和 SVG，无外部脚本、字体或图像依赖。`docs/preview.png` 为该组件的合成教学模型截图，不包含患者影像或第三方临床图片。
