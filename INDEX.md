# 小红书冷启动 — Skill Index

> 从公开长文方法论整理而来，产出 6 个可执行 Agent Skills。
> 处理时间: 2026-07-07

## 关于这篇文章

- **作者**: 文子 (@Eejoylove)
- **发布时间**: 2026-07-06
- **一句话主旨**: 先从变现路径倒推账号，再用 Agent 把对标、记忆、选题、改稿、排期复盘串成小红书冷启动系统。
- **融合补充**: 已融合 yanliudreamer 小红书系列，并提取 dbskill 与 xhs-visual-director-skill 中适合小红书场景的内容诊断、标题、对标、共鸣、视觉导演和复盘模块。
- **整篇理解**: [BOOK_OVERVIEW.md](./BOOK_OVERVIEW.md)
- **精华长文**: [DIGEST.md](./DIGEST.md)
- **术语词典**: [GLOSSARY.md](./GLOSSARY.md)
- **融合说明**: [FUSION_NOTES.md](./FUSION_NOTES.md)
- **dbskill 提取说明**: [DBSKILL_EXTRACTION_NOTES.md](./DBSKILL_EXTRACTION_NOTES.md)
- **视觉导演融合说明**: [VISUAL_DIRECTOR_FUSION_NOTES.md](./VISUAL_DIRECTOR_FUSION_NOTES.md)

## Skill 列表

### 定位与对标

- [`xhs-monetization-backsolve`](./xhs-monetization-backsolve/SKILL.md) — 先确认 offer、变现路径、timing 和个人 IP 路线，再倒推账号定位、内容方向、视觉信任感和验证计划。
- [`xhs-low-follower-pattern`](./xhs-low-follower-pattern/SKILL.md) — 找低粉爆款样本，用点击率 × 停留时长 × 互动率、对标过滤、共鸣解码和视觉骨架拆出可迁移结构。

### 内容生产系统

- [`xhs-account-profile`](./xhs-account-profile/SKILL.md) — 建立账号档案、个人语言样本、可信主张、视觉身份和长期记忆。
- [`xhs-topic-bank`](./xhs-topic-bank/SKILL.md) — 用七类标题公式、标题触发器、五类用户底层需求和封面钩子建立可持续选题库。

### 发布与迭代

- [`xhs-humanize-compliance`](./xhs-humanize-compliance/SKILL.md) — 对 AI 初稿做人味化、单一核心机制、5 秒开头、图文拆页和平台表达检查。
- [`xhs-schedule-review`](./xhs-schedule-review/SKILL.md) — 制定前 10 条/30 天排期，并把内容生产、视觉生产和 10-20 条数据复盘写回账号档案。

## 引用图

```mermaid
graph LR
    A["xhs-monetization-backsolve"] --> B["xhs-low-follower-pattern"]
    A --> C["xhs-account-profile"]
    B --> D["xhs-topic-bank"]
    C --> D
    D --> E["xhs-humanize-compliance"]
    E --> F["xhs-schedule-review"]
    F ==> D
    F ==> C
```

## 推荐使用顺序

1. `xhs-monetization-backsolve`
2. `xhs-account-profile`
3. `xhs-low-follower-pattern`
4. `xhs-topic-bank`
5. `xhs-humanize-compliance`
6. `xhs-schedule-review`

## 安装使用

把每个 skill 目录复制到你正在用的 Agent 的 skills 目录后重启即可，例如：

```bash
cp -R xhs-* ~/.codex/skills/    # Codex
cp -R xhs-* ~/.claude/skills/   # Claude Code
```

## 审计轨迹

- 候选单元池: [candidates/](./candidates/)
- 被淘汰候选: [rejected/](./rejected/)
- 阶段 0: [BOOK_OVERVIEW.md](./BOOK_OVERVIEW.md)
