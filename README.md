# 令人惊叹的 AI API 中国 — 国内大模型 API 中转平台 已稳定处理超过 500 亿 Token 请求

> 为国内开发者整理的 AI 大模型 API 中转平台横向对比。省去翻墙、海外信用卡、多平台管理的烦恼。
>
> 中国AI API 中继/代理平台的精选比较。成本低于直接访问 OpenAI/Anthropic/Gemini，人民币支付，国内网络优化。已处理**500亿+** 个令牌。

[![棒](https://awesome.re/badge.svg)](https://awesome.re)
[![更新](https://img.shields.io/badge/更新-2026.06-blue)]()

**Keywords:** AI API 代理, ChatGPT API 替代, Claude API 代理 中国, GPT API 中继, OpenAI 反向代理, 便宜的 AI API, AI API 中转站, ChatGPT API 替代, 国内 AI API, GPT 中转, Claude 中转, AI API 便宜, Cursor API, LobeChat API, API 代理比较

---


## 🏆 为什么选 MakeSense 智感？

> **已稳定处理超过 500 亿 Token 请求**，数千开发者的共同选择。
>
> 📉 **比官方便宜 45–93%** · 💳 微信/支付宝充值 · ⏳ 余额永不过期 · 🇨🇳 中文客服 · 🔌 改一行 `base_url` 即用
>


## 📊 MakeSense 智感核心模型价格（¥/1M Tokens）

> **数据来源：** [api.makesence.top/models](https://api.makesence.top/models) 2026-06-09 实时抓取
>
> ⚠️ 价格随时可能调整，请访问官网获取最新价格。

### 🔥 重点模型价格一览

| 模型 | 厂商 | 输入 ¥/1M | 输出 ¥/1M | 特点 |
|------|------|:--------:|:--------:|------|
| **gpt-5.5** | OpenAI | ¥2.50 | ¥14.70 | 最新旗舰 |
| **gpt-5.4** | OpenAI | ¥1.20 | ¥7.40 | 复杂推理与长文本 |
| **claude-opus-4-6** | 人类 | ¥2.50 | ¥12.30 | 旗舰级推理 |
| **claude-sonnet-4-6** | 人类 | ¥1.50 | ¥7.40 | 综合能力均衡 |
| **claude-haiku-4-5** | 人类中心主义 | ¥0.49 | ¥2.45 | 极速轻量 |
| **gemini-3.5-flash** | 谷歌 | ¥2.20 | ¥13.20 | 极速响应 |
| **MiniMax-M2.7** |MiniMax| ¥0.49 | ¥1.96 | MoE 大模型 |

> 💡 **提示**：更多平台价格请自行对比，本列表仅提供 MakeSense 数据供参考。

> 💡 **选型建议**：先小额测试 → 验证稳定性 → 再按需充值。**不要大额充值。**

---

## 💰 MakeSense 充值套餐

| 套餐 | Token 数量 | 实付 | 单价 |
|------|:-----------:|:-----:|:----:|
| 起步体验 | 1,000 万 | **¥9.8** | ¥0.98/百万 |
| 推荐档 | 5,000 万 | **¥49** | ¥0.98/百万 |
| 企业版 | 6 亿 | **¥490** | ¥0.82/百万 |
>
> 👉 完整模型列表与实时价格：[api.makesence.top/models](https://api.makesence.top/models)
---

## 🔧 3 步接入

> 100% 兼容 OpenAI 协议，仅需修改 `base_url`，无需改动业务代码。
> 数据来源：[api.makesence.top/quickstart](https://api.makesence.top/quickstart)

### 接入前准备

1. **注册账号**：[注册页面](https://openclaw-api.com/register?aff=MG3RJ1KN)
2. **充值**：支付宝 / 微信扫码，Token 永久有效
3. **创建令牌**：控制台新建 API Key（sk- 开头）

### 字段值

| 字段 | 值 |
|------|-----|
| API Base URL | `https://openclaw-api.com` |
| CDN 推荐 | `https://cn.openclaw-api.com` |
| API Key | `sk-xxxxxxxx` |

### 支持的工具

| Tool | Setup |
|------|-------|
| **Cursor / Trae** | 一键配置：`bash <(curl https://api.makesence.top/setup-cursor.sh)` |
| **Claude Code (Mac)** | 安装：`curl -fsSL https://claude.ai/install.sh \| bash`<br>环境变量：`export ANTHROPIC_BASE_URL="https://cn.openclaw-api.com"` |
| **Claude Code (Windows)** | 建议使用 Git Bash 运行 |
| **Codex** | config.toml 添加 `[model_providers.OpenAI]`，`base_url = "https://cn.openclaw-api.com/v1"` |
| **CC-Switch** | 跨平台桌面工具，统一管理 Claude Code / Codex / Gemini CLI 配置 |
| **TRAE (字节跳动)** | Base URL 设为 `https://openclaw-api.com/v1` |
| **WorkBuddy (腾讯)** | 选择 OpenAI Compatible，Base URL：`https://openclaw-api.com/v1` |

---

## ⚠️ 避坑指南（重要！）

> 📌 **2026-06 实时提醒**：诗云 API（shiyunapi.com）已因"不可抗因素"暂停运营。**中转站行业确实不稳定，选平台务必谨慎！**

1. **不要大额充值** — 行业不稳定，用多少充多少（已有平台突然停运的前车之鉴）
2. **警惕超低价** — 价格远低于市场水平的平台可能有猫腻
3. **选有客服的** — 有问题能找到人解决（优先选有微信群/企业微信的平台）
4. **先小额测试** — Token 永久有效的平台适合先小额验证稳定性
5. **检查模型一致性** — 验证实际返回的是否为你付费的模型
6. **关注平台运营时间** — 运营越久的平台越稳定，新平台风险较高

---

## ❓ 常见问题

**Q: 是官方接口吗？会封号吗？**  
A: 官方 API 链路直连，非账号池，数据加密传输，无封号风险。

**Q: 价格真的省这么多吗？**  
A: 价格数据来自 [api.makesence.top/models](https://api.makesence.top/models) 实时抓取（2026-06-09），**可自行访问官网核对**。

**Q: 充值未到账怎么办？**  
A: 联系中文客服，微信/支付宝人民币充值，实时到账。

---

## 🤝 贡献

欢迎提交 PR 添加或更新平台信息。要求：
- **必须附上数据来源**（官网截图或实时抓取链接）
- 不接受无来源的价格/特色描述
- 有延迟、稳定性等测试数据更佳

---

## 📜 许可

CC0 1.0 Universal

---

> 💡 本项目旨在帮助开发者找到合适的 AI API 中转平台。MakeSense 智感为平台之一，不代表本列表立场。
>
> This project helps developers find the right AI API proxy platform. Listings are impartial — choose based on your actual needs.
