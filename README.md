# Surge Rules 📡

一套为 Surge 用户设计的高效规则配置，专注于分流优化、广告拦截与隐私保护。

## ✨ 功能特点

- 🚀 智能分流（国内 / 国外流量自动判断）
- 🛑 广告拦截（过滤常见广告域名）
- 🔒 隐私保护（屏蔽追踪器）
- 🎯 自定义规则（支持扩展）
- ⚡ 高性能（精简规则，低延迟）

---

## 📦 目录结构

```
.
├── rules/
│   ├── direct.list
│   ├── proxy.list
│   ├── reject.list
│   └── apple.list
├── modules/
│   └── adblock.sgmodule
└── README.md
```

---

## 🚀 使用方法

### 方法一：远程规则引用（推荐）

在 Surge 配置文件中添加：

```ini
[Rule]
RULE-SET,https://your-domain.com/rules/direct.list,DIRECT
RULE-SET,https://your-domain.com/rules/proxy.list,PROXY
RULE-SET,https://your-domain.com/rules/reject.list,REJECT
```

---

### 方法二：模块导入

```ini
[Module]
https://your-domain.com/modules/adblock.sgmodule
```

---

## ⚙️ 规则说明

| 文件名        | 说明 |
|--------------|------|
| direct.list  | 国内直连 |
| proxy.list   | 代理访问 |
| reject.list  | 广告拦截 |
| apple.list   | Apple 服务优化 |

---

## 🧠 策略建议

- `DIRECT`：国内网站
- `PROXY`：Google / YouTube / AI 服务
- `REJECT`：广告 & 统计

---

## 🔄 更新说明

- 每周维护更新
- 持续优化规则
- 欢迎提交 Issue / PR

---

## 📌 兼容性

- ✅ Surge (iOS / macOS)
- ⚠️ Clash / Quantumult X 需转换格式

---

## 🤝 贡献

欢迎提交：

- 新规则
- Bug 修复
- 优化建议

---

## ⚠️ 免责声明

本项目仅供学习与研究使用，请遵守当地法律法规。

---

## ⭐ 支持

如果这个项目对你有帮助，欢迎 Star ⭐！