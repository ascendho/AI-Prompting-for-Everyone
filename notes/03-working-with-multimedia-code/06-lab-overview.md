# 06. Lab overview: Building with AI + final project

> **一句话核心**：M3 的 Lab 是**两个 1 小时的编程实验**——Building with AI（搭 app） + Final project（用 M1+M2+M3 全部工具做一个有实际价值的项目）。

## 📌 关键概念

- **Lab 1: Building with AI** = 把 [04-building-apps](./04-building-apps.md) 串成代码：用 AI 帮你写一个 app。
- **Lab 2: Final project** = 课程压轴 — **综合 M1+M2+M3** 做一个你真正用得上的项目。
- 这两个 Lab 不在课件 PDF 里（在 DeepLearning.AI 平台），课件只到"Data analysis"为止。
- Final project 的意义：**学完三个模块后，证明你真的能"用 AI 做事"**。

## 🧪 Lab 1: Building with AI

### 目标

从 **GOAL/INPUT/OUTPUT 三块积木** 出发，用 AI 生成一个**最小可运行**的 app。

### 典型做法

```python
# 伪代码
prompt = """
GOAL: A simple flashcard app for learning French
INPUT: User types a French word
OUTPUT: App shows the English translation + a "Next" button
Stack: HTML + CSS + JavaScript (no backend)
"""

# 步骤 1: 让 AI 生成代码
app_code = call_ai(prompt)

# 步骤 2: 让 AI 解释关键部分
explained = call_ai("Explain the code you just wrote, line by line")

# 步骤 3: 迭代改进
v2 = call_ai("""
Now add:
  - A 'Don't know' button that shows the answer
  - Track correct/incorrect count
  - Reset button
""")
```

### 练习选题（参考 [04-building-apps](./04-building-apps.md) 难度谱）

| 难度 | 选题 |
|---|---|
| 🟢 Easy | Pomodoro timer / bill calculator / flashcard / outfit picker |
| 🟡 Medium | Chain reaction game / fireworks（已演示） |
| 🔴 Hard | 实时法语对话练习 / 多人对战游戏 |

**建议** Lab 1 选 🟢 Easy，做"能跑通"的小 app 就行。

## 🧪 Lab 2: Final project

### 目标

把 **M1 + M2 + M3 全部能力** 用在一个你**真的用得上**的项目上。

### Final project 的 4 大方向

| 方向 | M1 | M2 | M3 | 例子 |
|---|---|---|---|---|
| **研究类** | ✅ Web search / Deep research | ✅ Brainstorm / Writing | | "对比 3 个保险方案优劣" |
| **写作类** | ✅ Web search | ✅ Progressive outlining / Critique | ✅ Image generation | "写一篇带配图的周报" |
| **App 类** | | ✅ Brainstorm | ✅ Building apps | "做一个个人待办 app" |
| **数据类** | | ✅ Critique | ✅ Data analysis | "分析我上个月的支出" |

### 选题的 4 条铁律（来自课件精神）

1. **用得上** — 别做"作业项目"，做"我会天天用的"
2. **至少用到 2 个模块的能力** — 否则不算综合
3. **不要追求完美** — 第一次跑通就够
4. **记录过程** — Lab 里写的 prompt 和迭代值得保留

### 选题模板

```text
我想做一个 [项目类型]，目标用户是 [谁]，
要解决 [具体痛点]。

会用到的能力：
  - [ ] M1: Pretrained / Web search / Deep research
  - [ ] M2: Brainstorm / Context / Sycophancy / Writing / Critique
  - [ ] M3: Image understanding / Image generation / App / Data analysis

成功标准（任选 1-2 条）：
  - [可量化指标] e.g. 节省 1 小时/周
  - [可观察行为] e.g. 我会连续用 3 次
```

## 🎯 Lab 隐藏的 4 个学习目标

| 目标 | 在 Lab 里怎么做 |
|---|---|
| 1. **M1+M2+M3 综合应用** | 选一个**至少跨 2 个模块**的项目 |
| 2. **迭代 prompt** | 第一版 → 反馈 → 第二版 → 反馈 → ... |
| 3. **判断"够好就停"** | 别陷入"再改改"陷阱 |
| 4. **记录你的 prompt** | 你的 prompt 库是长期资产 |

## ⏭ Module 3 Quiz 准备建议

Lab 做完后再去做 [Module 3 Quiz](https://www.deeplearning.ai/courses/ai-prompting-for-everyone/lesson/bvllku83/module-3-quiz)，重点复盘：

| 主题 | 关键 |
|---|---|
| [01-multimedia-overview](./01-multimedia-overview.md) | 6×6 in/out 矩阵 + 速度/成本谱 + 责任 |
| [02-image-understanding](./02-image-understanding.md) | 3 条 recap tips（读文字 / 漏细节 / 多图） |
| [03-image-generation](./03-image-generation.md) | 3 要素 prompt + diffusion 3 大错误 + 慢且贵 |
| [04-building-apps](./04-building-apps.md) | GOAL/INPUT/OUTPUT 积木 + 难度谱 |
| [05-data-analysis](./05-data-analysis.md) | AI 写+跑代码 + 何时触发 code tool |

## 🎓 整门课学完之后

| 模块 | 主题 | 现在的能力 |
|---|---|---|
| M1 | Finding Information | 知道 AI 怎么"找信息"，能用 3 种工具精准问问题 |
| M2 | AI as a Thought Partner | 能让 AI 跟你 brainstorm、帮你写、给你真批评 |
| M3 | Working with Multimedia & Code | 能用 AI 看图、画图、建 app、分析数据 |

> **最终能力**：把 AI 当**通用助理**——任何日常任务（写邮件、做报表、查资料、想方案、做 app）都有可用套路。

---

> 下一节 [recap: Multimedia & Code 总览 + 5 大能力卡片 + 决策流程图](./recap.md)；自测题见 [practice/03-working-with-multimedia-code.md](../../practice/03-working-with-multimedia-code.md)。
