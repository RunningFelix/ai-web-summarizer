# ai-web-summarizer
# AI 网页内容总结（增强版）

这是一个结合了 AI 技术的增强版油猴脚本，用于总结网页内容。该脚本通过调用 OpenAI 兼容的 API，自动提取并总结当前网页的主要观点、关键信息和重要细节，并以美观的 Markdown 格式呈现结果。

## 功能特性

* **一键总结:** 通过简单的按钮点击或自定义快捷键（默认 Alt+S）触发总结功能。
* **界面友好:** 提供简洁易用的用户界面。
* **自定义设置:**  提供设置面板，允许用户自定义 API 配置信息，包括：
    * API 地址
    * API 密钥
    * 模型类型
    * 最大 Token 数量
    * **总结提示词:**  允许用户自定义用于指导 AI 总结的提示词，以获得更精准的结果。
* **多配置管理 (v1.4):** 支持保存、加载和切换多个 API 参数设置。
* **拖拽贴靠与位置保存 (v1.4):** 支持拖拽总结窗口并保存其位置。
* **下载总结功能 (v1.5):**  允许用户下载总结结果为 Markdown 文件。
* **增强 macOS 快捷键兼容性 (v1.5):** 提升了 macOS 系统下的快捷键兼容性。
* **优化拖动和贴靠体验 (v1.5):**  改进了拖动和贴靠的流畅度。
* **Markdown 渲染与配置管理修复 (v1.5):**  修复了 Markdown 渲染和配置管理相关的问题。
* **AI 驱动:** 利用 AI 技术，提供更准确和高效的网页内容总结。
* **CSP 和 CORS 跨域问题解决 (v1.6):** 解决了内容安全策略 (CSP) 和跨域资源共享 (CORS) 相关问题，提高了脚本稳定性。
* **Bug 修复和稳定性提升 (v1.6):**  修复了多个 bug 并进行了多项改进，增强了脚本的可靠性。
* **预定义提示词模板(v1.7):**  新增多种预定义提示词模板，方便用户快速选择合适的提示词；

## 安装

1. 安装油猴脚本管理器，例如 Tampermonkey 或 Greasemonkey。
2. 从 [Greasy Fork 链接](https://greasyfork.org/zh-CN/scripts/515734-ai%E7%BD%91%E9%A1%B5%E5%86%85%E5%AE%B9%E6%80%BB%E7%BB%93-%E5%A2%9E%E5%BC%BA%E7%89%88) 安装脚本。

## 使用

1. 导航到要总结的网页。
2. 点击“总结网页”按钮或使用配置的快捷键（默认为 Alt+S）。
3. 总结结果将显示在一个模态窗口中。您可以复制总结、将其下载为 Markdown 文件或使用不同的设置重试总结。


## 许可证

* **v1.5 及更早版本：** MIT 许可证
* **v1.6 及以后版本：** Apache 2.0 许可证  (详见 [LICENSE](LICENSE.txt) 文件)


## 贡献

欢迎贡献！请提交 issue 或 Pull Request。


## 版本更新日志

* **v1.7:** 新增多种预定义提示词模板，方便用户快速选择合适的提示词；支持配置重命名，方便用户管理配置。
* **v1.6:** 解决了 CSP 和 CORS 跨域问题，修复了多个 bug，并提升了整体脚本稳定性。  更改许可证为 Apache 2.0。
* **v1.5:** 增强了 macOS 系统的快捷键兼容性，增加了下载总结功能，优化了拖动和贴靠体验，修复了 markdown 渲染和配置管理的问题，复制的格式改为 markdown，提升了用户体验和脚本稳定性。
* **v1.4:** 增加了多配置保存、加载和切换功能，实现了拖拽贴靠和保存容器位置的功能。
* **v1.2:** 通过使用 Shadow DOM、增强快捷键和移动端支持、优化设置面板和复制功能、改进错误处理和代码结构等方式，显著提升了用户体验、代码质量和稳定性。


**(可选) 测试专用 API (不保证稳定性):**

虽然建议您使用自己的 OpenAI API 密钥，但以下提供了一个测试 API（不保证稳定性）：

* **地址:** `https://snowy-forest-7d66.ttjmggm.workers.dev/v1/chat/completions`
* **密钥:** `sk-fortest123`

**注意:** 此 API 仅供测试使用。为了获得更可靠的解决方案，请获取您自己的 OpenAI API 密钥。 更多API信息请参考以下链接：[AI总结网页脚本，附测试专用api](https://linux.do/t/topic/250373)  (需要 Linux.do 账号，Lv1 以上等级)。该链接会不定时更新 API 信息。 *请注意，第三方 API 的可用性和功能不在本项目的控制范围内。*