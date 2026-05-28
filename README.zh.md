# Skills 技能库

AI Agent 技能库 — 模块化、可复用的 Claude Code / Codex 能力扩展。

---

## 📋 技能目录

### 🧘 个人效率

| 技能 | 说明 | 适用场景 |
|------|------|---------|
| [method-gtd](method-gtd/) | **GTD** — Getting Things Done 搞定 | 任务堆积、事务繁多，需要一个可靠系统清空大脑 |
| [method-pomodoro](method-pomodoro/) | **番茄工作法** — 专注时间与休息循环 | 拖延症、注意力分散、需要结构化专注 |
| [method-eisenhower-matrix](method-eisenhower-matrix/) | **四象限法则** — 紧急×重要优先级矩阵 | 整天救火、任务过载、需要决定放弃哪些事 |
| [method-atomic-habits](method-atomic-habits/) | **原子习惯** — 微小改变复合效应 | 新年决心从未坚持、想要持久的自我改变 |
| [method-eat-the-frog](method-eat-the-frog/) | **吃青蛙** — 最难的事优先做 | 重要的事总被拖延、早上精力最充沛 |
| [method-time-blocking](method-time-blocking/) | **时间块管理** — 日历预定整块时间 | 整天被动响应、深度工作不断被推到"之后" |
| [method-bullet-journal](method-bullet-journal/) | **子弹笔记** — 符号化手账系统 | 喜欢手写记录、现有工具太僵化、想要可自由定制的系统 |
| [method-pareto](method-pareto/) | **二八法则 (80/20)** — 80%效果来自20%投入 | 优先级过多、资源有限、需要找到高杠杆环节 |

### 🧠 问题分析与决策

| 技能 | 说明 | 适用场景 |
|------|------|---------|
| [method-5why-3how](method-5why-3how/) | **5Why + 3How** — 根因分析 + 对策制定 | 问题重复发生、需从3个维度深挖根因并制定系统对策 |
| [method-pdca](method-pdca/) | **PDCA 循环** — 计划-执行-检查-改进 | 流程优化、质量管理、需要系统性验证改进效果 |
| [method-first-principles](method-first-principles/) | **第一性原理** — 回归基本面重建 | 创新瓶颈、行业假设值得怀疑、需要突破性方案 |
| [method-inversion](method-inversion/) | **逆向思维** — 反向思考避免失败 | 过度乐观的计划、高风险决策需要识别盲点 |
| [method-six-thinking-hats](method-six-thinking-hats/) | **六顶思考帽** — 平行思维切换 | 团队意见冲突、需要结构化的多视角讨论 |
| [method-ooda](method-ooda/) | **OODA 循环** — 观察-定向-决策-行动 | 竞争激烈、对手行动快、需要快速适应变化 |
| [method-mece](method-mece/) | **MECE 原则** — 相互独立完全穷尽 | 复杂问题分解、分析报告框架搭建、数据分类 |

### 🏢 团队与规划

| 技能 | 说明 | 适用场景 |
|------|------|---------|
| [method-agile](method-agile/) | **敏捷开发** — Scrum / Kanban / XP | 需求不断变化、需要快速反馈和频繁交付 |
| [method-okr](method-okr/) | **OKR** — 目标与关键成果 | 季度/年度规划、跨团队对齐、需要富有挑战的目标 |
| [method-smart](method-smart/) | **SMART 原则** — 目标设定准则 | 制定清晰可衡量的目标、项目里程碑定义 |
| [method-moscow](method-moscow/) | **MoSCoW 优先级法** — Must/Should/Could/Won't | MVP 范围界定、待办项过多需要明确排出放弃项 |
| [method-swot](method-swot/) | **SWOT 分析** — 优劣势/机会/威胁 | 战略规划、产品发布前评估、个人职业规划 |
| [method-design-thinking](method-design-thinking/) | **设计思维** — 以人为本的创新方法 | 新产品的用户需求探索、模糊问题需要结构化方法 |
| [method-rice](method-rice/) | **RICE 打分法** — Reach/Impact/Confidence/Effort | 不同类型项目难比较、各方都说"这是最高优先级" |

---

## 🚀 使用方法

```bash
# 克隆仓库
git clone https://github.com/ihgoa501-stack/skills.git

# 安装单个技能到 Claude
ln -s "$(pwd)/method-gtd" ~/.claude/skills/method-gtd

# 或一次性安装全部
for d in $(ls -d method-*); do ln -sf "$(pwd)/$d" ~/.claude/skills/"$d"; done
```
