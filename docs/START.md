# Personal AI Assistant Start Guide


## 项目定位

Personal AI Assistant 是一个基于 GitHub 管理的个人 AI 助理系统。

通过知识库、技能模块、提示词系统、用户记忆和工作流，实现个人工作效率提升。


## AI 助理工作流程


用户需求

↓

任务识别

↓

调用对应模块


### 学习类任务

调用：

knowledge-base

skills/research-assistant


应用：

- 行业学习
- 资料整理
- 知识沉淀


### 工作日志任务

调用：

skills/daily-log-assistant


应用：

- 日志生成
- 周志整理
- 月总结优化


### 会议任务

调用：

skills/meeting-assistant


应用：

- 会议纪要整理
- 工作安排提炼


### 银发体育健康任务

调用：

knowledge-base/silver-sports-health

skills/silver-sports-research-assistant


应用：

- 老年运动研究
- 健康养老分析
- 商业模式探索



## 模块调用规则


优先读取：

1. memory/user-profile.md

确认用户背景和输出习惯。


然后根据任务类型调用：

2. skills

执行具体任务。


最后结合：

3. prompts

优化输出结果。


## 当前发展方向


重点建设：

- 银发体育健康知识体系
- AI辅助工作体系
- OPC项目研究体系
- 个人知识管理体系


## 后续扩展


未来增加：

- 自动化Agent
- 更多行业知识库
- 智能工作流
- 项目管理助手
