# Skills

AI Agent skills collection — modular, reusable capability extensions for Claude Code and Codex.

## Directory

| Skill | Description | 适用场景 |
|-------|-------------|---------|
| [method-gtd](method-gtd/) | GTD — Getting Things Done | 任务堆积、事务繁多、需要一个可靠系统清空大脑 |
| [method-pomodoro](method-pomodoro/) | 番茄工作法 — 专注时间与休息循环 | 拖延症、注意力分散、需要结构化专注 |
| [method-5why](method-5why/) | 5WHY 分析法 — 根因追溯 | 故障复盘、问题重复发生、从表象深挖到底层 |
| [method-pdca](method-pdca/) | PDCA 循环 — 持续改进 | 流程优化、质量管理、需要系统性验证改进效果 |
| [method-okr](method-okr/) | OKR — 目标与关键成果 | 季度/年度规划、跨团队对齐、需要富有挑战的目标 |
| [method-smart](method-smart/) | SMART 原则 — 目标设定准则 | 制定清晰可衡量的目标、项目里程碑定义 |
| [method-eisenhower-matrix](method-eisenhower-matrix/) | 四象限法则 — 紧急×重要优先级 | 整天救火、任务过载、需要决定哪些事该放弃 |
| [method-agile](method-agile/) | 敏捷开发 — Scrum / Kanban / XP | 需求不断变化的产品开发、需要快速反馈迭代 |
| [method-atomic-habits](method-atomic-habits/) | 原子习惯 — 微小改变复合效应 | 习惯养成失败、想要持久的自我改变 |
| [method-first-principles](method-first-principles/) | 第一性原理 — 回归基本面 | 创新瓶颈、行业假设值得怀疑、需要突破性方案 |
| [method-inversion](method-inversion/) | 逆向思维 — 反向思考避免失败 | 过度乐观的计划、需要识别盲点的高风险决策 |
| [method-six-thinking-hats](method-six-thinking-hats/) | 六顶思考帽 — 平行思维切换 | 团队意见冲突、需要结构化的会议讨论 |
| [method-ooda](method-ooda/) | OODA 循环 — 观察-定向-决策-行动 | 竞争激烈的环境、危机响应、需要快速适应变化 |
| [method-pareto](method-pareto/) | 二八法则 — 80%效果来自20%投入 | 优先级过多、资源有限、需要找到高杠杆环节 |
| [method-eat-the-frog](method-eat-the-frog/) | 吃青蛙 — 最难的事优先做 | 重要的事情一直被拖延、早上效率最高 |
| [method-time-blocking](method-time-blocking/) | 时间块管理 — 日历预定时间 | 整天在被动响应、重要工作被推到"之后" |
| [method-moscow](method-moscow/) | MoSCoW 优先级法 — Must/Should/Could/Won't | MVP 范围界定、待办项过多、需要明确排出放弃项 |
| [method-bullet-journal](method-bullet-journal/) | 子弹笔记 — 符号化手账系统 | 喜欢手写记录、现有工具过于僵化、想要可自由定制的系统 |
| [method-swot](method-swot/) | SWOT 分析 — 优劣势/机会/威胁 | 战略规划、产品发布前评估、个人职业规划 |
| [method-mece](method-mece/) | MECE 原则 — 相互独立完全穷尽 | 复杂问题分解、分析报告框架搭建、数据分类 |
| [method-design-thinking](method-design-thinking/) | 设计思维 — 以人为本的创新 | 新产品的用户需求探索、模糊问题需要结构化方法 |
| [method-rice](method-rice/) | RICE 打分法 — Reach/Impact/Confidence/Effort | 不同类项目难比较、请求方都说"这是最高优先级" |

## Usage

```bash
# Clone the repo
git clone https://github.com/ihgoa501-stack/skills.git

# Symlink or copy a skill into your Claude skills directory
ln -s "$(pwd)/work-methodology" ~/.claude/skills/work-methodology
```
