# 文子的小红书工作流

![文子的小红书工作流：从定位到复盘的六个 Agent Skills](./assets/hero-xhs-workflow.png)

> 文子的小红书 Agent Skills：让 Agent 帮你跑完整套小红书冷启动，从定位、选题、改稿、图文规划，到发布排期和数据复盘。

这不是“再写一篇小红书文案”的提示词合集，而是一套可以安装到 **Codex / Claude Code / Cursor 及其他支持 Agent Skills 的工具** 的内容运营工作流。

你只需要告诉 Agent：

```text
我想做一个面向职场新人的 AI 工具号，未来通过咨询变现。
请带我从定位开始，建立账号档案，并规划前 10 条内容。
```

它会依次帮你交付：

1. 一句话账号定位与变现路径
2. 可长期复用的账号档案
3. 低粉高数据样本拆解
4. 35+ 个结构化选题与标题
5. 前 10 条及 30 天发布计划
6. 单篇内容的人味化改稿与 6–8 页图文结构
7. 每周数据复盘与下一轮实验

## 真实结果不是口号

这套方法来自真实的小红书内容实践。下面展示的是过往阅读与互动结果，用来说明工作流经过实际运营验证；每个账号的基础、选题和执行情况不同，因此这些案例不代表对粉丝数或流量的承诺。

<p align="center">
  <img src="./assets/proof-500k-reads.png" alt="小红书笔记累计阅读超过 50 万" width="38%">
  <img src="./assets/proof-engagement.png" alt="小红书点赞收藏、关注与评论反馈" width="58%">
</p>

## 60 秒开始

### 1. 安装

这套 Skill 不绑定某一个 AI 产品。把 6 个 `xhs-*` 目录复制到你正在用的 Agent 的 skills 目录即可：

```bash
# Codex
cp -R xhs-* ~/.codex/skills/

# Claude Code
cp -R xhs-* ~/.claude/skills/

# 其他支持 Agent Skills 的工具：复制到对应 skills 目录后重启
```

完成后重启对应应用。将 `SKILL.md` 放入支持 Agent Skills 的工作台即可使用。

### 2. 直接说人话，不必记 Skill 名

**从零起号**

```text
我想做小红书，但还不知道定位和变现方式。请先帮我盘点优势和可售卖资产，再规划前 10 条内容。
```

**已有账号重新梳理**

```text
这是我过去发布的内容和数据。请判断定位是否需要收敛，并给出下一轮 10 条内容的测试计划。
```

**单篇内容优化**

```text
这篇初稿 AI 味太重。请保留我的真实观点，把它改成能直接发布的小红书文案，并拆成 8 页图文结构。
```

## 它不是一次性写作工具

```text
变现倒推定位
→ 建立账号档案
→ 规划前 10 条系统画像内容
→ 生成选题库和标题
→ 校准初稿与图文结构
→ 学习低粉高数据样本
→ 用 10–20 条数据复盘定位
→ 把结论写回账号档案
```

每一轮发布都会留下数据和结论，成为下一轮内容的输入。目标不是让 AI 替你批量生产“营销号文案”，而是逐步建立一套更像你、也更懂你账号的内容系统。

## 你会得到什么

### 输入

```text
我是一名文科生，日常高频使用 AI 做写作和知识管理。
我想服务“想用 AI 提升效率、但不懂技术”的职场人。
未来希望通过咨询和课程变现。
我不想做夸张营销，也不公开承诺收益。
```

### 输出

- **定位卡**：帮谁、解决什么问题、为什么相信你
- **变现路径**：主路径、副路径、内容如何建立信任
- **账号档案**：语气、真实经历、可信主张、内容与视觉边界
- **选题库**：痛点、数字、对比、稀缺、共鸣、资源、反常识七类选题
- **内容计划**：前 10 条、7 天或 30 天发布节奏
- **单篇成稿**：标题、开头、正文、互动点、图文拆页
- **复盘报告**：有效假设、失效假设、下周调整动作

## 6 个 Skills

| 你现在的问题 | Skill | 核心交付 |
|---|---|---|
| 不知道做什么账号，也不知道未来卖什么 | `xhs-monetization-backsolve` | 变现路径、定位卡、内容矩阵、10–20 条验证计划 |
| 每次让 AI 写内容，都不像你本人 | `xhs-account-profile` | 账号档案、语言样本、可信主张、内容与视觉边界 |
| 想拆低粉高数据样本为什么有效 | `xhs-low-follower-pattern` | 样本筛选、点击/停留/互动诊断、可迁移结构 |
| 缺选题、标题和封面钩子 | `xhs-topic-bank` | 35+ 选题、标题公式、封面方向、发布优先级 |
| 初稿太顺、太空、太像模板 | `xhs-humanize-compliance` | AI 味诊断、真人化改稿、发布检查、图文拆页 |
| 不知道前 10 条怎么发，或发完不会复盘 | `xhs-schedule-review` | 发布排期、数据看板、定位复盘、下周实验 |

## 三种推荐工作流

### 从 0 开始做新号

```text
xhs-monetization-backsolve
→ xhs-account-profile
→ xhs-low-follower-pattern
→ xhs-topic-bank
→ xhs-humanize-compliance
→ xhs-schedule-review
```

### 已有账号重新梳理

```text
xhs-schedule-review
→ xhs-monetization-backsolve
→ xhs-account-profile
→ xhs-low-follower-pattern
→ xhs-topic-bank
```

### 单篇内容优化

```text
xhs-topic-bank
→ xhs-humanize-compliance
→ xhs-low-follower-pattern
```

## 设计原则

### 先定商业方向，再做内容

没有清楚的目标用户、信任资产和 offer，选题越多越容易把账号做散。定位 Skill 会先回答：谁为什么需要你、为什么相信你、内容如何承接下一步关系。

### 学结构，不复制表达

优先分析近期、低粉、高数据的样本，拆解封面承诺、标题、开头、正文结构、收藏理由和评论动机。迁移的是内容机制，不是原文。

![搜索关键词并按最新排序，寻找低粉高数据样本](./assets/demo-low-follower-search.png)

*示例：搜索垂直关键词并切换到“最新”，从近期内容里寻找可分析的真实样本。*

### 真人感来自证据，不是口语词

“去 AI 味”不只是把句子写得随意，而是加入真实经历、具体场景、踩坑、数据、对话和前后变化。

### 用一轮数据修正定位

前 10–20 条是验证期，不因为一篇数据高就立刻复制，也不因为三篇数据低就过早放弃。每周把结论写回账号档案，再决定下一轮测试什么。

## 项目结构

```text
.
├── README.md
├── INDEX.md
├── BOOK_OVERVIEW.md
├── DIGEST.md
├── FUSION_NOTES.md
├── DBSKILL_EXTRACTION_NOTES.md
├── VISUAL_DIRECTOR_FUSION_NOTES.md
├── GLOSSARY.md
├── verified.md
├── candidates/
├── rejected/
├── xhs-monetization-backsolve/
├── xhs-low-follower-pattern/
├── xhs-account-profile/
├── xhs-topic-bank/
├── xhs-humanize-compliance/
└── xhs-schedule-review/
```

每个 Skill 目录包含：

- `SKILL.md`：Agent 可调用的技能说明
- `test-prompts.json`：触发、边界和回归测试用例

更多内部说明：

- [INDEX.md](./INDEX.md)：技能依赖关系与推荐顺序
- [BOOK_OVERVIEW.md](./BOOK_OVERVIEW.md)：对原文方法论的理解与批判
- [DIGEST.md](./DIGEST.md)：方法精华
- [DBSKILL_EXTRACTION_NOTES.md](./DBSKILL_EXTRACTION_NOTES.md)：dbskill 模块的提取与转译
- [VISUAL_DIRECTOR_FUSION_NOTES.md](./VISUAL_DIRECTOR_FUSION_NOTES.md)：视觉导演方法的融合说明
- [verified.md](./verified.md)：已核验的方法论单元
- [rejected/](./rejected/)：未纳入 Skill 的建议及原因

## 方法来源

项目以文子的 X Article《别不信！WorkBuddy 就可以把你的小红书从 0 粉干到 1000》为冷启动主线，并融合：

- [原始 X Article](https://x.com/Eejoylove/status/2074028317498601870)
- yanliudreamer 小红书系列中的起号、个人 IP、内容验证和长期增长方法
- [dontbesilent2025/dbskill](https://github.com/dontbesilent2025/dbskill/tree/main) 中适合小红书运营的标题、内容诊断、对标、共鸣、开头、文风和复盘模块
- [ziguishian/xhs-visual-director-skill](https://github.com/ziguishian/xhs-visual-director-skill) 中适合图文内容的视觉导演方法

本仓库只保留短引用、方法论重写和可执行工作流，不包含来源文章全文。

## 使用边界

- Skill 提供的是内容运营方法和决策支持，不保证粉丝数、流量或变现结果。
- 平台规则、推荐机制和工具能力会变化，发布前仍应结合当前规则核验。
- “养号”“特定设备流量更好”等缺少稳定证据的说法没有被写入执行流程。
- 拆解对标内容时只学习结构、机制和用户需求，不复制原文或侵犯他人权益。

## 下一步计划

- 增加统一入口 Skill，让新手不必先判断应该调用哪一个模块
- 增加账号档案、选题库、30 天排期和复盘看板模板
- 为 Codex 增加更友好的中文展示名称和默认提示词
- 建立可自动执行的触发测试和行为回归测试

欢迎提交 Issue 或 Pull Request，分享真实使用结果和需要补充的场景。
