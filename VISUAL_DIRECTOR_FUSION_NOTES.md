# 视觉导演融合说明

更新时间: 2026-07-07

本次参考 [ziguishian/xhs-visual-director-skill](https://github.com/ziguishian/xhs-visual-director-skill)，把其中适合小红书冷启动系统的视觉导演方法提取到现有 `workbuddy-xhs-skills`。处理方式不是把视觉导演 skill 整包并入，而是把它转译成现有 6 个小红书运营 skills 的视觉交付字段。

## 提取的核心模块

| 视觉导演模块 | 提取内容 | 落到本项目 |
|---|---|---|
| 10 问澄清 | 完整图文项目前先明确目标、受众、观点、素材、风格、转化 | `xhs-humanize-compliance`, `xhs-schedule-review` |
| 风格判断报告 | 判断内容类型、传播目标、读者情绪、信息密度、推荐风格 | `xhs-topic-bank`, `xhs-account-profile` |
| 3 套风格方案 | 点击优先、收藏优先、高级感/个人品牌优先 | `xhs-topic-bank`, `xhs-monetization-backsolve` |
| 8 页结构 | 封面、痛点、认知、方法、案例、操作、总结、引导 | `xhs-humanize-compliance`, `xhs-schedule-review` |
| 统一视觉母版 | 1080x1440px、3:4、边距、网格、字体、色彩、组件语言 | `xhs-account-profile`, `xhs-schedule-review` |
| 视觉审查清单 | 封面冲击、手机端可读、信息层级、风格统一、避免 PPT 感 | `xhs-humanize-compliance`, `xhs-low-follower-pattern` |
| 视觉数据复盘 | 记录封面风格、主视觉、页数、收藏反馈、视觉失效原因 | `xhs-schedule-review`, `xhs-account-profile` |

## 融合后的变化

### 1. 选题不只看标题

`xhs-topic-bank` 现在要求优先选题补充视觉字段:

- 内容类型
- 传播目标
- 读者情绪
- 信息密度
- 封面钩子
- 主视觉方向
- 推荐风格
- 页数建议

这样选题可以继续交给视觉导演生成 3:4 封面或 6-8 页图文。

### 2. 改稿可以拆成图文

`xhs-humanize-compliance` 增加图文页面结构和视觉可读性检查。用户要发图文时，不再把长文硬塞进页面，而是拆成封面、痛点、认知、方法、案例、操作、总结、引导。

### 3. 对标要拆视觉骨架

`xhs-low-follower-pattern` 增加封面构图、信息层级、主视觉、页间节奏、母版一致性和手机端可读性等字段。学习样本时只提取结构，不复制原作者专属素材。

### 4. 账号档案增加视觉身份

`xhs-account-profile` 增加视觉身份字段:

- 默认画幅
- 主风格和辅助风格
- 色彩令牌
- 字体系统
- 封面标题比例
- 内页组件
- 图标/线条语言
- 禁用视觉反模式

### 5. 排期包含视觉生产

`xhs-schedule-review` 不只安排发布时间，还安排图文制作任务，包括 10 问澄清、视觉母版、视觉确认图、最终图和审查时间。

### 6. 定位阶段加入视觉信任感

`xhs-monetization-backsolve` 增加视觉定位假设。不同变现路径对应不同视觉信任感: 咨询和企业服务要专业可信，教程和工具要清晰可收藏，个人 IP 要形成可持续视觉识别。

## 保持的边界

- 本项目仍是 Agent XHS Skills，不替代独立的 XHS Visual Director Skill。
- 需要真正生成图片时，仍应使用专门的视觉生成工具或视觉导演 skill。
- 本项目负责把“内容运营流程”接上“视觉交付字段”，让选题、正文、排期和复盘都能自然进入图文生产。
