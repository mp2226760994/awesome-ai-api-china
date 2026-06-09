# GitHub 提 PR/Issue + 自建仓库 完整行动计划

## 🎯 目标
1. 在已有的 AI API 汇总仓库中插入 api.makesence.top
2. 自建 `awesome-ai-api-china` 仓库作为独立推广阵地

---

## ✅ 已完成

| 事项 | 文件 | 状态 |
|------|------|------|
| awesome-ai-api-china README | `awesome-ai-api-china/README.md` | ✅ 已写好 |
| whataicc/ai-proxy Issue 草稿 | `issues/issue-whataicc-ai-proxy.md` | ✅ 已写好 |
| zzsting88/relayAPI Issue 草稿 | `issues/issue-zzsting88-relayAPI.md` | ✅ 已写好 |

---

## ⏳ 待完成（需要 GitHub 登录）

### 1. 创建 awesome-ai-api-china 仓库
```bash
cd awesome-ai-api-china
git init
git add README.md
git commit -m "feat: 国内AI API中转平台汇总"
gh repo create awesome-ai-api-china --public --source=. --remote=origin --push
```

### 2. 给 whataicc/ai-proxy 提 Issue
```bash
gh issue create --repo whataicc/ai-proxy \
  --title "[建议] 添加 MakeSense 智感 (api.makesence.top) 到推荐列表" \
  --body-file issues/issue-whataicc-ai-proxy.md
```

### 3. 给 zzsting88/relayAPI 提 Issue 或通过 hvoy.ai 提交
```bash
# 方案A: GitHub Issue
gh issue create --repo zzsting88/relayAPI \
  --title "[新增推荐] MakeSense 智感 api.makesence.top" \
  --body-file issues/issue-zzsting88-relayAPI.md

# 方案B: hvoy.ai 提交（手动访问 https://www.hvoy.ai/contact）
```

### 4. 补充搜索更多 API 汇总仓库
```bash
# 搜索可以提 Issue 的其他仓库
gh search repos "API中转" --topic awesome-list
```

---

## 📊 预期效果

| 渠道 | 预期流量 | 生效周期 |
|------|---------|---------|
| GitHub awesome-ai-api-china | SEO 长尾，月均 50-200 点击 | 1-2 周 |
| zzsting88/relayAPI 推荐 | 直接推荐流量 | 添加后即时 |
| hvoy.ai 评测收录 | 评测 SEO 流量 | 1-2 周 |
| whataicc/ai-proxy | 不确定（可能是竞品拒绝） | 不确定 |