# 🚀 Surge Rule Sets

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/badge/Surge-Compatible-blue.svg)](https://nssurge.com/)
[![Last Update](https://img.shields.io/badge/Last_Update-2026--04-brightgreen.svg)]()

一个精简、高效、且实时更新的 Surge 规则集，旨在提供最丝滑的上网体验。

---

## 🌟 核心特色
- **极速响应**：基于 Domain Set 优化，在大规模规则下依然保持极低延迟。
- **精准分流**：细化流媒体、社交、开发工具及金融应用的分流逻辑。
- **去广告增强**：整合了隐私追踪屏蔽，深度净化网页与 App。
- **自动更新**：每日由脚本自动抓取并去重。

---

## 🛠 配置指南

### 1. 快速引入
将以下代码复制到你的 Surge 配置文件的 `[Rule]` 模块下方：

```text
# --- [My Rule Sets] ---
# 社交媒体 (Telegram, Twitter等)
RULE-SET,[https://raw.githubusercontent.com/YOUR_USER/Surge/main/Social.list,PROXY](https://raw.githubusercontent.com/YOUR_USER/Surge/main/Social.list,PROXY)

# 全球流媒体 (Netflix, Disney+等)
RULE-SET,[https://raw.githubusercontent.com/YOUR_USER/Surge/main/Streaming.list,Media](https://raw.githubusercontent.com/YOUR_USER/Surge/main/Streaming.list,Media)

# 广告拦截
RULE-SET,[https://raw.githubusercontent.com/YOUR_USER/Surge/main/AdBlock.list,REJECT](https://raw.githubusercontent.com/YOUR_USER/Surge/main/AdBlock.list,REJECT)

# 最终兜底
FINAL,DIRECT
