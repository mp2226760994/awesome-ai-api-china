# 🇨🇳 Awesome AI API China — 国内大模型 API 中转平台汇总

> 为国内开发者整理的 AI 大模型 API 中转平台横向对比。省去翻墙、海外信用卡、多平台管理的烦恼。

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![更新](https://img.shields.io/badge/更新-2026.06-blue)]()

---

## 📌 为什么需要 API 中转？

- 🚫 **官方接口国内不稳定**：OpenAI / Anthropic 接口经常超时、限流
- 💳 **支付门槛高**：需要海外信用卡、外币结算
- 🔑 **多平台管理繁琐**：GPT、Claude、Gemini 各一套 Key
- 💰 **官方价格贵**：中转平台通常有折扣渠道

**中转平台 = 统一接口 + 国内加速 + 人民币支付 + 折扣价格**

---

## 📊 主流平台横向对比

| 平台 | 起步价 | GPT-5.5 价格 (输入/输出 /M tokens) | Claude Opus 价格 (输入/输出 /M tokens) | 模型覆盖 | 支付方式 | 特色 |
|------|--------|-------------------------------------|----------------------------------------|---------|---------|------|
| **[MakeSense 智感](https://api.makesence.top)** | ¥9.8/1000万 | ¥1.2 / ¥7.2 | ¥10 / ¥50 | GPT/Claude/Gemini/DeepSeek等50+ | 微信/支付宝 | 官方直连不掺水，OpenAI协议兼容，<50ms延迟 |
| [神马中转](https://api.whatai.cc) | — | ¥1.5 / ¥9 | ¥11 / ¥55 | GPT/Claude/Gemini/Suno/Midjourney | 微信/支付宝 | 模型覆盖广，支持AI绘图 |
| [诗云API](https://shiyunapi.com) | — | ¥1.3 / ¥7.8 | ¥9.5 / ¥47.5 | GPT/Claude/Gemini | 微信/支付宝 | 延迟极低20ms，SLA 99.92% |
| [4SAPI](https://4sapi.com) | — | ¥1.5 / ¥9 | ¥10.5 / ¥52.5 | GPT/Claude/Gemini/国产 | 微信/支付宝 | 企业级稳定性，多重冗余 |
| [PoloAPI](https://poloapi.com) | — | ¥1.4 / ¥8.4 | ¥10 / ¥50 | GPT/Claude/Gemini | 微信/支付宝 | UI好看，独立开发者友好 |
| [BAYLLM](https://bayllm.com) | — | ¥1.3 / ¥7.8 | ¥9.8 / ¥49 | GPT/Claude/Gemini | 微信/支付宝 | Cursor/Claude Code 深度适配 |
| [PackyCode](https://packycode.com) | ¥50起 | ¥2.5 / ¥15 | ¥10 / ¥50 | GPT/Claude/Gemini | 微信/支付宝 | 开源社区活跃，开发票 |
| [DeRouter](https://derouter.com) | — | ¥1.5 / ¥9 | ¥11 / ¥55 | GPT/Claude/Gemini | 银行卡/USDT | P2P 订阅共享模式 |
| [OpenRouter](https://openrouter.ai) | — | 按官方价+5% | 按官方价+5% | 全球所有模型 | 海外卡/USDT | 最全模型覆盖，原厂直连 |

> ⚠️ 价格会随行情波动，以上为 2026.06 参考价。建议少量充值测试后再决定。

---

## 🎯 选型指南

### 个人开发者 / 轻度用户
→ **[MakeSense 智感](https://api.makesence.top)** ¥9.8 起，无最低消费，Token 永久有效，最适合体验和轻量工具

### 日常 AI 编程（Cursor / Claude Code / Windsurf）
→ **[MakeSense 智感](https://api.makesence.top)** 或 [BAYLLM](https://bayllm.com)，OpenAI 协议改 base_url 即用

### 企业级高并发
→ [4SAPI](https://4sapi.com) 或 [诗云API](https://shiyunapi.com)，SLA 保障

### 需要 AI 绘图
→ [神马中转](https://api.whatai.cc)，支持 Midjourney / Suno

---

## 🔧 如何接入（通用流程）

所有中转平台都兼容 OpenAI 协议，接入只需改 `base_url`：

```python
# Python 示例
import openai

openai.api_key = "你的API Key"
openai.api_base = "https://api.makesence.top"  # 或任意中转平台地址

response = openai.ChatCompletion.create(
    model="gpt-4o",
    messages=[{"role": "user", "content": "你好"}]
)
```

**支持的工具：**

| 工具 | 配置方式 |
|------|---------|
| Cursor | Settings → Models → 添加 OpenAI API Key + Base URL |
| Claude Code | `claude --api-key xxx --base-url https://api.makesence.top` |
| LobeChat | 设置 → 语言模型 → OpenAI → 自定义接口地址 |
| Chatbox / NextChat | 设置 → API Host → 填入中转站地址 |
| QQ 机器人（Napcat） | application.yml 中配置 api-key 和 api-base |

---

## ⚠️ 避坑指南

1. **不要大额充值**：行业不稳定，用多少充多少
2. **警惕超低价**：GPT-5.5 低于 ¥0.8/M token 的基本掺水
3. **优先选有群/有客服的**：跑路风险真实存在
4. **实测缓存价格**：正常缓存价应该是原价 10%，黑心站收 30%+
5. **检查模型一致性**：请求 GPT 返回的是不是 GPT，有些站拿国产模型冒充

---

## 🤝 贡献

如果你是 API 中转站站长或用户，欢迎提 PR 添加/更新平台信息。

提交要求：
- 提供平台名称、URL、价格、模型覆盖等基本信息
- 如有评测数据（延迟、稳定性等）更佳
- 不接受虚假/夸大宣传

---

## 📜 许可

CC0 1.0 Universal — 自由使用、修改、分发。

---

> 💡 本项目旨在帮助国内开发者找到适合自己的 AI API 方案。排名不分先后，请根据实际需求选择。