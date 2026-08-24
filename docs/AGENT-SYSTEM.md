# Agent System Guide


## 系统定位

Personal AI Assistant 通过多个 Agent 协同完成不同类型任务。

整体架构：

用户需求

↓

Router Agent

↓

任务分类

↓

调用对应 Agent

↓

调用 Skills

↓

输出结果


---

# Agent 架构


## 1. Router Agent

文件：

agents/router-agent.md


职责：

负责识别用户需求，并分配任务。


触发：

所有任务首先经过 Router Agent。


示例：

用户：

"帮我生成今天日志"


判断：

日志任务


调用：

Daily Log Agent



---

# 2. Daily Log Agent


文件：

agents/daily-log-agent.md


职责：

负责：

- 日志生成
- 周志整理
- 月总结


调用：

skills/daily-log-assistant


适用场景：

工作记录

学习总结

成长复盘



---

# 3. Silver Sports Health Agent


文件：

agents/silver-sports-agent.md


职责：

负责银发体育健康领域研究。


调用：

knowledge-base/silver-sports-health


适用：

- 老年运动研究
- 健康养老分析
- 运动方案设计
- 市场研究



---

# 4. OPC Incubation Agent


文件：

agents/opc-incubation-agent.md


职责：

负责项目孵化分析。


适用：

- 项目评估
- 商业模式设计
- 产品规划
- 落地方案设计



---

# Agent 调用规则


## 工作类任务

流程：

Router Agent

↓

Daily Log Agent

↓

daily-log-assistant



---

## 行业研究任务

流程：

Router Agent

↓

Silver Sports Health Agent

↓

知识库


---

## 项目孵化任务

流程：

Router Agent

↓

OPC Incubation Agent

↓

商业分析模块



---

# 数据读取优先级


第一层：

memory

读取用户背景。


第二层：

knowledge-base

读取专业知识。


第三层：

skills

执行具体任务。


第四层：

prompts

优化输出。


---

# 输出原则


所有 Agent 输出遵循：


1. 结合用户实际背景

2. 注重结果价值

3. 提供可执行方案

4. 避免空泛内容

5. 保持长期知识沉淀



---

# 当前系统版本


Version:

V1.0


持续迭代。
