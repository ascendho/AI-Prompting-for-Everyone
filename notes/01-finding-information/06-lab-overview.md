# 06. Lab overview: AI model prompt comparison

> **一句话核心**：Module 1 的 Lab 是一个 1 小时的编程实验，让你在代码里**同时调用多个 AI 模型**，直观比较它们的回答。

## 📌 关键概念

- 课程提供了一个**代码示例**（Code Example，约 1 小时），不是测验。
- Lab 的设计意图：把第 1-5 节学到的工具——**预训练知识、Web search、Deep research**——**用代码**串起来。
- 它的核心是 **prompt comparison**：同一 prompt 跑多个模型，看输出差异。

## 🧪 Lab 在做什么

课件说明该实验的目的是**对比不同 AI 模型对相同 prompt 的反应**：

- 同样的问题给 GPT-4o、Claude、Gemini、Llama 等不同模型
- 打开/关闭 web search
- 打开/关闭 deep research
- 改变 prompt 措辞（length / context / rubric）观察输出变化

> 注意：Lab **不要求你精通** Python 编程，但建议能读懂简单的 API 调用。

## 🛠 实际玩法（基于课件的精神）

### Step 1：选一个值得对比的 prompt

挑一个你最近在 **02-05** 节里练习过的真实问题，例如：

- 「Pros and cons of taking peptides as a supplement?」
- 「Find me a highly rated gym near Mountain View, CA」
- 「What are the tradeoffs for each car? Read everything and think hard before answering」

### Step 2：构造对比矩阵

```python
# 伪代码
models = ["gpt-4o", "claude-sonnet-4.5", "gemini-2.5-pro"]
modes  = ["pretrained", "web_search", "deep_research"]
prompts = {
    "novice": "Tell me about peptides.",
    "power_user": """Compare the pros and cons of taking peptides
                     as a supplement. Only use sources from official
                     health organizations. Provide inline citations."""
}

for model in models:
    for mode in modes:
        for p_name, p in prompts.items():
            response = call_api(model, mode, p)
            print(f"== {model} | {mode} | {p_name} ==")
            print(response)
            print("-" * 60)
```

### Step 3：记录你看到的差异

| 对比维度 | 观察点 |
|---|---|
| **信源选择** | 哪个模型默认拉到更权威的信源？ |
| **时效性** | 涉及最新事件时谁更准？ |
| **结构化** | 谁更爱用表格/列表？ |
| **批判性** | 哪个更敢指出 prompt 本身的漏洞？ |
| **deep research 循环深度** | 哪个能搜到 50+ 源？哪个 5 个就交差？ |

## 🎯 Lab 的隐藏目标

> 课件没明说，但通过对比你能练出**两条**关键能力：

1. **选模型的直觉** — 不同任务该用哪个模型，下次不用反复试。
2. **写更好的 prompt** — 看完 6 个 (model × mode) 矩阵格，你会立刻知道**短 prompt 是浪费**。

## ⏭ Module 1 Quiz 准备建议

Lab 做完后再去做 [Module 1 Quiz](https://www.deeplearning.ai/courses/ai-prompting-for-everyone)，重点复盘：

- 3 个工具的**对比表**（见 [recap.md](./recap.md)）
- 5 个 novice vs power user 场景（见 [01](./01-novice-vs-power-user.md)）
- Web search 4 步流程（见 [04](./04-web-search-sources.md)）

---

> 下一节 [recap: 总览 + 三大工具对比 + 决策流程图 + Quiz 自测](./recap.md)
