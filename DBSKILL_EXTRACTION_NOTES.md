# dbskill 提取说明

更新时间: 2026-07-07

本次没有把小红书 skills 并入 dbskill，也没有让本仓库依赖 dbskill 的运行入口。处理方式是：阅读 dbskill 中与内容增长、标题、对标、共鸣、开头、文风和复盘有关的模块，把其中适合小红书冷启动的判断框架转译到现有 `xhs-*` skills。

参考项目:

- [dontbesilent2025/dbskill](https://github.com/dontbesilent2025/dbskill/tree/main)

## 提取模块

| dbskill 模块 | 提取内容 | 落到本仓库 |
|---|---|---|
| `dbs-xhs-title` | 标题公式可追溯、12 类心理触发器、20 字以内、保留悬念、真实痛点、至少 2 个张力元素 | `xhs-topic-bank` |
| `dbs-content` | 内容质量四维诊断、产品/服务先于内容、不要只堆干货 | `xhs-humanize-compliance`, `xhs-monetization-backsolve` |
| `dbs-benchmark` | 对标五重过滤: 商业相关、机制可懂、可复用、剔除主观噪音、少空谈赛道 | `xhs-low-follower-pattern` |
| `dbs-resonate` | 单一核心机制、共鸣五维诊断、内容为什么让人想表达或转述 | `xhs-humanize-compliance`, `xhs-low-follower-pattern` |
| `dbs-spread` | 从样本反推传播原因，而不只拆结构 | `xhs-low-follower-pattern`, `xhs-topic-bank` |
| `dbs-hook` | 5 秒开头独立成立: 话题、继续看的理由、可信证据 | `xhs-humanize-compliance` |
| `dbs-ai-check` | 先诊断再改写，识别太顺、太满、太正确的 AI 文风 | `xhs-humanize-compliance`, `xhs-account-profile` |
| `dbs-save / restore / report` 思路 | 每周结论写回账号档案，形成下一轮实验输入 | `xhs-schedule-review`, `xhs-account-profile` |

## 转译后的变化

### 1. 选题库更重视标题质量

`xhs-topic-bank` 不再只是按七类标题方向生成候选，而是要求每个标题标注来源类型，并通过五项硬检:

- 20 个中文字符以内
- 保留悬念，不把答案说完
- 用更大的用户词，而不是过窄行业词
- 击中真实痛点
- 至少包含 2 个张力元素

### 2. 改稿先诊断再润色

`xhs-humanize-compliance` 增加:

- 内容四维诊断
- 单一核心机制审计
- 5 秒开头检查
- 个人证据补强

它的目标不是把文字改得更花，而是判断这篇内容到底卡在标题承诺、表达效率、证据、结构还是真人感。

### 3. 对标先过滤再学习

`xhs-low-follower-pattern` 增加五重对标过滤，避免用户只学习数据好看的样本。保留下来的样本必须和账号目标有关，且能被拆成用户自己的素材。

同时增加共鸣解码: 样本让用户想评论、收藏或转述，是因为它释放了某种表达、满足了某个使用动机，还是提供了一个可站队的框架。

### 4. 定位先看 offer

`xhs-monetization-backsolve` 增加 offer 与信任路径检查。用户不能只说“以后变现”，而要先写清:

- 产品、服务或资源是什么
- 谁为什么需要
- 凭什么信任
- 内容如何自然承接下一步关系

### 5. 复盘要写回记忆

`xhs-schedule-review` 增加周度运营报告，要求把有效假设、失效假设、强标题类型、强内容机制、下周实验写回账号档案。这样每周复盘不是聊天里的临时结论，而是下一轮选题和改稿的输入。

### 6. 账号档案要有个人语言和可信主张

`xhs-account-profile` 增加两个关键字段:

- 个人语言样本: 用户真实会说的话、不会说的话、常用句式和情绪边界
- 可信主张清单: 可以公开主张什么、有什么证据、哪些结果不能承诺、哪些 offer 可以被内容承接

## 设计边界

- 本仓库仍是 Agent XHS Skills，不是 dbskill 分支。
- dbskill 的通用商业诊断入口没有被复制进来，只提取对小红书运营有用的判断模块。
- 所有模块都落在现有 `xhs-*` skill 里，保持“小红书冷启动工作流”的清晰边界。
