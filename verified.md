# Verified Method Units

## F01 变现倒推账号定位

```yaml
id: F01
title: 变现倒推账号定位
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 文章开头强调先确定产品和变现方式
    - 结尾再次强调先想清楚变现再做账号
V2_predictive_power:
  passed: true
  novel_question: "如果用户想做读书账号但不知道发什么，下一步是什么？"
  derived_answer: "先确认读书账号靠课程、社群、咨询、带货还是广告变现，再反推内容栏目。"
V3_exclusivity:
  passed: true
  why_not_common: "常识是先发内容找感觉；这里要求先确定商业路径再做内容。"
```

## F02 低粉爆款拆解

```yaml
id: F02
title: 低粉爆款拆解
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 文章单独给出搜索、排序、筛选、改写四步
    - 后文要求把 5-10 篇样本交给 Agent 拆规律
V2_predictive_power:
  passed: true
  novel_question: "新手做职场成长号没有素材，应该先看大号还是低粉爆款？"
  derived_answer: "先看低粉爆款，因为它更能说明内容结构本身有效。"
V3_exclusivity:
  passed: true
  why_not_common: "不是泛泛参考竞品，而是用低粉高数据样本降低粉丝基础干扰。"
```

## F03 账号档案

```yaml
id: F03
title: 账号档案
type: principle
V1_cross_domain:
  passed: true
  evidence:
    - 文章要求建立账号档案
    - 后文强调记忆文件是核心资产
V2_predictive_power:
  passed: true
  novel_question: "为什么同一个提示词生成的内容总是不像我？"
  derived_answer: "缺少长期账号档案，工具不知道定位、边界和语气。"
V3_exclusivity:
  passed: true
  why_not_common: "重点不是写简介，而是把账号信息变成可跨会话读取的协作记忆。"
```

## F04 七类选题库

```yaml
id: F04
title: 七类选题库
type: framework
V1_cross_domain:
  passed: true
  evidence:
    - 文章列出七类小红书标题方向
    - 后文要求按类型生成多组标题公式
V2_predictive_power:
  passed: true
  novel_question: "每天不知道发什么，是否应该让 AI 自由想题？"
  derived_answer: "不应自由发挥，应先用类型公式库约束方向。"
V3_exclusivity:
  passed: true
  why_not_common: "它把灵感问题改造成模板填空和组合问题。"
```

## F05 去 AI 味与规则检查

```yaml
id: F05
title: 去 AI 味与规则检查
type: checklist
V1_cross_domain:
  passed: true
  evidence:
    - 文章第六步要求加个人口吻
    - 同段强调平台规则检查
V2_predictive_power:
  passed: true
  novel_question: "一篇初稿结构完整但读起来很普通，下一步不是重写，而是什么？"
  derived_answer: "先加真实经历和具体细节，再检查表达边界。"
V3_exclusivity:
  passed: true
  why_not_common: "不是简单润色，而是人格化和发布风险检查的组合流程。"
```

## F06 排期复盘闭环

```yaml
id: F06
title: 排期复盘闭环
type: workflow
V1_cross_domain:
  passed: true
  evidence:
    - 文章要求 30 天三阶段排期
    - 后文要求每周记录数据并沉淀规律
V2_predictive_power:
  passed: true
  novel_question: "发布三篇后不知道下一篇怎么改，应该问什么？"
  derived_answer: "把曝光、点击、收藏、评论等数据放进复盘表，让下一周选题来自数据。"
V3_exclusivity:
  passed: true
  why_not_common: "不是普通日历，而是把节奏、类型和数据判断连成闭环。"
```

