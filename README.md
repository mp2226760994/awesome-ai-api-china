# 🇨🇳 Awesome AI API China — 国内大模型 API 中转平台汇总 | AI API Proxy Comparison China

> 为国内开发者整理的 AI 大模型 API 中转平台横向对比。省去翻墙、海外信用卡、多平台管理的烦恼。
> 
> A curated comparison of AI API proxy/relay platforms in China. Alternative to direct OpenAI/Anthropic/Gemini API access with lower cost, CNY payments, and domestic network optimization.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![更新](https://img.shields.io/badge/更新-2026.06-blue)]()

---

**Keywords / 关键词:**  
AI API proxy, ChatGPT API alternative, Claude API proxy China, GPT API relay, OpenAI reverse proxy, cheap AI API, AI API 中转站, ChatGPT API 替代方案, 国内 AI API, GPT 中转, Claude 中转, AI API 便宜, Cursor API alternative, LobeChat API, API proxy service comparison, best AI API proxy 2026

---

## 📌 为什么需要 API 中转？ | Why Use an API Proxy?

- 🚫 **官方接口国内不稳定**：OpenAI / Anthropic 接口经常超时、限流
- 💳 **支付门槛高**：需要海外信用卡、外币结算
- 🔑 **多平台管理繁琐**：GPT、Claude、Gemini 各一套 Key
- 💰 **官方价格贵**：中转平台通常有折扣渠道

**中转平台 = 统一接口 + 国内加速 + 人民币支付 + 折扣价格**

---

## 📊 平台横向对比 | Platform Comparison

| 平台 Platform | 起步价 Min. | GPT-5.5 价格 Price (in/out per 1M tokens) | Claude Opus 价格 Price | 模型 Models | 支付 Payment | 特色 Features |
|------|--------|-------------------------------------|----------------------------------------|---------|---------|------|
| **[MakeSense 智感](https://api.makesence.top)** | ¥9.8 | ¥1.2 / ¥7.2 | ¥10 / ¥50 | GPT/Claude/Gemini/DeepSeek 50+ | 微信/支付宝 CNY | OpenAI protocol, <50ms latency |
| [神马中转 API Relay](https://api.whatai.cc) | — | ¥1.5 / ¥9 | ¥11 / ¥55 | GPT/Claude/Gemini/Suno/MJ | 微信/支付宝 | 650+ models, image gen |
| [诗云 ShiyunAPI](https://shiyunapi.com) | — | ¥1.3 / ¥7.8 | ¥9.5 / ¥47.5 | GPT/Claude/Gemini | 微信/支付宝 | ~20ms latency |
| [4SAPI](https://4sapi.com) | — | ¥1.5 / ¥9 | ¥10.5 / ¥52.5 | GPT/Claude/Gemini/CN | 微信/支付宝 | Enterprise SLA |
| [PoloAPI](https://poloapi.com) | — | ¥1.4 / ¥8.4 | ¥10 / ¥50 | GPT/Claude/Gemini | 微信/支付宝 | Dev-friendly UI |
| [BAYLLM](https://bayllm.com) | — | ¥1.3 / ¥7.8 | ¥9.8 / ¥49 | GPT/Claude/Gemini | 微信/支付宝 | Cursor/Claude Code ready |
| [PackyCode](https://packycode.com) | ¥50 | ¥2.5 / ¥15 | ¥10 / ¥50 | GPT/Claude/Gemini | 微信/支付宝 | Open source community |
| [DeRouter](https://derouter.com) | — | ¥1.5 / ¥9 | ¥11 / ¥55 | GPT/Claude/Gemini | Bank/USDT | P2P subscription |
| [OpenRouter](https://openrouter.ai) | — | Official+5% | Official+5% | All global models | Intl cards/USDT | Widest model coverage |

> ⚠️ Prices may fluctuate. Test with small top-up before committing.

---

## 🎯 选型指南 | Which Platform to Choose?

### 个人开发者 / Individual Developers
→ **[MakeSense 智感](https://api.makesence.top)** — ¥9.8 minimum, no expiry, best for trying out

### AI 编程工具 / AI Coding Tools (Cursor / Claude Code / Windsurf)
→ **[MakeSense 智感](https://api.makesence.top)** or [BAYLLM](https://bayllm.com) — OpenAI protocol, change base_url and go

### 企业高并发 / Enterprise High Concurrency
→ [4SAPI](https://4sapi.com) or [诗云API](https://shiyunapi.com) — SLA guaranteed

### AI 绘图 / AI Image & Music Generation
→ [神马中转](https://api.whatai.cc) — Midjourney / Suno support

---

## 🔧 快速接入 | Quick Setup

All platforms support OpenAI protocol. Just change `base_url`:

```python
import openai

openai.api_key = "your-api-key"
openai.api_base = "https://api.makesence.top"  # or any proxy URL

response = openai.ChatCompletion.create(
    model="gpt-4o",
    messages=[{"role": "user", "content": "Hello"}]
)
```

**Supported tools:**

| Tool | Setup |
|------|-------|
| [Cursor](https://cursor.sh) | Settings → Models → OpenAI API Key + Base URL |
| [Claude Code](https://claude.ai) | `claude --api-key xxx --base-url https://api.makesence.top` |
| [LobeChat](https://lobechat.com) | Settings → Language Model → OpenAI → Custom API URL |
| [NextChat](https://nextchat.fun) | Settings → API Host → proxy URL |
| Chatbox | Settings → API Host → proxy URL |

---

## ⚠️ 避坑指南 | Tips & Warnings

1. **不要大额充值** — Don't top up large amounts; the industry is volatile
2. **警惕超低价** — Suspiciously cheap prices may mean model substitution
3. **选有客服的** — Prefer platforms with active support/community
4. **检查模型一致性** — Verify you're actually getting the model you pay for
5. **先小额测试** — Always test with minimum top-up first

---

## 🤝 贡献 | Contribute

PRs welcome to add or update platform info. Requirements:
- Platform name, URL, pricing, model coverage
- Benchmark data (latency, uptime) preferred
- No false/exaggerated claims

---

## 📜 许可 | License

CC0 1.0 Universal

---

> 💡 本项目旨在帮助开发者找到适合自己的 AI API 方案。排名不分先后，请根据实际需求选择。
> 
> This project helps developers find the right AI API proxy platform. Listings are impartial — choose based on your needs.