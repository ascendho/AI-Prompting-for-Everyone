# 08. Lab overview: Brainstorming and critique with AI

> **一句话核心**：M2 的 Lab 把 01-07 的内容**串成一个 1 小时的编程实验**：在代码里跑**头脑风暴 + rubric 评估**的完整流程。

## 📌 关键概念

- Lab 的设计意图：把"对话式"的 brainstorming + critique 翻译成**可重复、可对比的代码流程**。
- 实验包含两部分：
  - **头脑风暴** — 调用多个模型生成多个方案。
  - **Rubric 评估** — 用一个详细 rubric 评估方案，或让另一个模型评估。
- 不需要深度编程，**重点是观察"不同模型 + 不同 prompt"对结果的差异**。

## 🧪 Lab 在做什么

课件说明该实验的目的是把 M2 的核心技巧——**brainstorming、context、sycophancy、writing、critique**——用代码跑通。

### 典型实验结构（基于课件精神）

```python
# 伪代码
import openai
import anthropic
import google.generativeai as genai

# === Part 1: Brainstorming across models ===
problem = "Help me plan a 12-month runway for a 4-person AI startup with $500K cash."

models = {
    "gpt-4o":  openai_client,
    "claude":  anthropic_client,
    "gemini":  genai,
}

context_prompt = """
Context:
- 4 founders, technical
- $500K cash, 18-month target runway
- Building developer tools

Task: Give 3 distinct plans, ranging from conservative to bold.
For each: key actions, expected runway, biggest risk.
"""

# Each model gives 3 plans
brainstorm_results = {m: call(m, context_prompt, n=3) for m in models}

# === Part 2: Cross-model critique with rubric ===
# Let Model A brainstorm, let Model B evaluate with a detailed rubric
output_for_review = brainstorm_results["gpt-4o"][0]  # take GPT-4o's Plan 1

rubric = generate_rubric_with_ai(
    "For a 12-month startup plan, design a 100-point rubric with "
    "4-5 dimensions, each with 3-5 specific criteria."
)

critique = call("claude", f"""
Critique this plan using the rubric below.
For each criterion, give a score and quote the plan text.

Plan:
{output_for_review}

Rubric:
{rubric}
""")
```

## 🎯 Lab 隐藏的 4 个学习目标

| 目标 | 在 Lab 里怎么做 |
|---|---|
| 1. **迭代 brainstorming** | 让每个模型跑 3 轮（生成 → 反馈 → 重新生成） |
| 2. **用好 context** | 对比"有 context" vs "没 context" 的输出差异 |
| 3. **识别 sycophancy** | 对比"leading prompt" vs "neutral prompt" 的评分差异 |
| 4. **用 rubric 评估** | 对比"详细 rubric" vs "模糊 rubric" 的评分差异 |

## 🛠 实际玩法

### 实验 1：Brainstorming 跨模型对比

| 维度 | 观察点 |
|---|---|
| **选项数量** | 哪个模型默认给最多方案？ |
| **选项差异** | 三个选项之间是否真正不同？ |
| **质量** | 哪个模型的"Plan 1"最像真正能用的？ |
| **响应时间** | 哪个最快？ |

### 实验 2：Context 的影响

- 同 prompt，A 组没 context，B 组带 6 个上下文
- 看输出**是否变得具体**

### 实验 3：Sycophancy 验证

- 让 3 个模型**给同一篇糟糕短文评分**
- 不用 rubric，看是否都"客客气气"打了 80+ 分
- 加上 rubric，看分数**是否合理下降**

### 实验 4：Rubric 设计

- 让 AI 设计 rubric
- 用 AI 设计的 rubric 去评分
- 跟"模糊 rubric"对比

## ⏭ Module 2 Quiz 准备建议

Lab 做完后再去做 [Module 2 Quiz](https://www.deeplearning.ai/courses/ai-prompting-for-everyone/lesson/3sxxzzl3/module-2-quiz)，重点复盘：

- **Brainstorming 配方**：Context → Options → Iteration（[01](./01-brainstorming.md)）
- **Context 三原则**：多≠好/相关才好/新话题开新对话（[02](./02-context.md)）
- **Desktop app 安全**：删除不进回收站（[03](./03-ai-desktop-apps.md)）
- **Reasoning 4 铁律**：最好模型/够 context/难任务/think hard（[04](./04-reasoning.md)）
- **Sycophancy 3 种应对**：中立措辞/显式批评/新对话（[05](./05-sycophancy.md)）
- **Writing 5 步法**：研究→大纲→修订→扩展→成文（[06](./06-writing.md)）
- **Rubric 评分**：好 rubric 的 2 个要素 + 跨模型审查（[07](./07-ai-critique.md)）

---

> 下一节 [recap: AI as a Thought Partner 总览 + 7 大原则 + 决策流程图](./recap.md)；自测题见 [practice/02-ai-as-thought-partner.md](../../practice/02-ai-as-thought-partner.md)。
