# Prompt 模板 · Module 2: AI as a Thought Partner

---

## 来自 [01. Brainstorming with AI](../notes/02-ai-as-thought-partner/01-brainstorming.md)

```text
模板 1: 标准头脑风暴（带上下文）
───────────────────
I'm trying to [目标].
My context: [你的具体背景/约束清单].
Give me 3-5 different approaches, ranging from conservative to creative.
For each, list the main idea, the trade-off, and an example.

模板 2: 迭代（反馈 + 重新生成）
───────────────────
Here are 3 options you gave me: [贴上 AI 上一轮的 3 个选项]
I like: [A 的某点 + B 的某点]
I don't like: [C 整体 / D 的某点]
New constraint that just came up: [新事实/约束]
Create 3 new options that combine what I liked with the new constraint.

模板 3: 探索"长尾创意"（避免常识答案）
───────────────────
Brainstorm 10 unusual/creative ways to [目标].
Skip the obvious answers (e.g., [列举 2-3 个太常见的答案]).
For each idea, briefly explain why it might work in my specific situation:
[1-2 句关于你的情况].

模板 4: 收口（选出最佳 → 落地）
───────────────────
Based on the options above, I prefer [选项编号] because [理由].
Now flesh it out into a step-by-step action plan I can start this week.
Include risks and what to do if step [X] doesn't work.
```

---

## 来自 [02. Context](../notes/02-ai-as-thought-partner/02-context.md)

```text
模板 1: 上传相关文件
───────────────────
I'm attaching:
  - [简历.pdf]  my background
  - [项目计划.xlsx]  current project status
  - [截图.png]  visual reference

Based on these, [具体任务]. Cite which file each recommendation comes from.

模板 2: 显式控制 context
───────────────────
For this question, only use the context I provide below.
Do NOT use your pretrained knowledge or assumptions.
If the context doesn't contain the answer, say so explicitly.

[粘贴 / 上传 context]

模板 3: 开新对话
───────────────────
[New chat]
Topic: [新话题]
Ignore any past conversation. Start fresh.
```

---

## 来自 [03. AI desktop apps](../notes/02-ai-as-thought-partner/03-ai-desktop-apps.md)

```text
模板 1: 整理文件
───────────────────
Analyze the folder [path]. Propose a plan to reorganize it.
DO NOT execute yet. Show me the plan first, including which files
will be moved/renamed/deleted.

模板 2: 跨文件总结
───────────────────
In [path], there are [N] files about [topic].
Read them as needed, then give me a 1-page summary covering:
  - Main themes
  - Disagreements between sources
  - Open questions

DO NOT modify any files.

模板 3: 批量处理（极小权限）
───────────────────
For each .docx file in [path] that contains "[keyword]":
  - Add a tag [tag-name] to the filename
  - Show me a list of what you changed BEFORE executing

模板 4: 备份优先
───────────────────
Before making any changes, copy [path] to [backup-path].
Then proceed with [task].
```

---

## 来自 [04. Reasoning with AI](../notes/02-ai-as-thought-partner/04-reasoning.md)

```text
模板 1: 显式要求深度思考
───────────────────
[复杂问题]

Take your time. Think through the problem step by step before answering.
Show your reasoning. Then give the final answer.

模板 2: Claude ultrathink 风格
───────────────────
[任务]
Ultrathink this. Consider multiple angles, edge cases, and tradeoffs.
Don't give me a quick answer—I want the deep version.

模板 3: 强制最新模型
───────────────────
Use the most capable model available. Budget is not a concern
for this task; quality is.

模板 4: 给齐上下文再让 AI 推理
───────────────────
Context:
  - [事实 1]
  - [事实 2]
  - [我的约束]

Question: [真问题]
Reason through this carefully. If anything in the context is
ambiguous or missing, ask me before answering.
```

---

## 来自 [05. Sycophancy](../notes/02-ai-as-thought-partner/05-sycophancy.md)

```text
模板 1: 显式中立 + 要反对意见
───────────────────
I'm considering [方案/想法/论点].

Don't take my framing as the truth. Present:
  - 2-3 strongest arguments FOR my position
  - 2-3 strongest arguments AGAINST
  - 1-2 alternative perspectives I might be missing

模板 2: 装成反对者
───────────────────
You are a skeptical [editor / investor / senior engineer].
Critique the following [文档/计划/代码] as if you want to reject it.
Be specific. List every weakness. Don't soften with "but overall…".

模板 3: 排除"礼貌"
───────────────────
Review this [essay / design / proposal].
Do NOT use phrases like "great job", "well done", or "interesting".
Start directly with the most important issue.

模板 4: 让 AI 自查
───────────────────
Review your previous answer. Identify any places where you
agreed with me just to be agreeable, rather than because the
evidence supports it. Be honest.
```

---

## 来自 [06. Writing with AI](../notes/02-ai-as-thought-partner/06-writing.md)

```text
模板 1: 反 AI slop 检查
───────────────────
Review this draft. Flag any of the following AI fingerprints:
  - Em dashes (—)
  - "Delve", "nuanced", "robust", "comprehensive"
  - Lists of three ("X, Y, and Z")
  - "Not just X, but Y" sentence patterns
  - Vague phrases like "change everything", "in today's world"
Rewrite the offending sentences in a more direct, human voice.

模板 2: 渐进式大纲（5 步合一）
───────────────────
Article topic: [topic]
My angle: [你的独特视角]
Counter-argument I want to address: [反对意见]
Stories/anecdotes I want to use: [1-2 个真实故事]

Step 1: Research 3-5 authoritative sources.
Step 2: Give me 3 different outline options.
Step 3: I'll pick + revise.
Step 4: Expand the revised outline into bullet points.
Step 5: I'll ask for prose.

Start with Step 1.

模板 3: 多风格探索
───────────────────
Here's a sentence I want to convey: [原句]

Rewrite it in 3 different voices:
  - Punchy (短促、有力)
  - Visionary (宏大、面向未来)
  - Conversational (口语化)

I'll mix-and-match.

模板 4: 大纲级编辑
───────────────────
Here's the current outline: [贴大纲]

If I change "[X]" to "[Y]", show me the updated outline
in full (not just the changed line).
```

---

## 来自 [07. AI critique](../notes/02-ai-as-thought-partner/07-ai-critique.md)

```text
模板 1: 让 AI 帮你设计 rubric
───────────────────
I'm going to evaluate [essay / design / code] for [purpose].
Propose a rubric with:
  - 4-6 dimensions
  - Each dimension: 3-5 specific scoring criteria with point values
  - Total = 100 points
Make each criterion checkable (yes/no or clear pass/fail).

模板 2: 严格的逐项评分
───────────────────
Here's the work to evaluate: [粘贴]
Here's the rubric: [粘贴模板 1 的输出]

For EACH criterion:
  - Score: [X] / [Y]
  - Quote the exact line(s) from the work that justify this score
  - If you can't quote anything, the score is 0

After all criteria, sum the scores. Do NOT round up.

模板 3: 显式反谄媚 prompt
───────────────────
Critique the following [work]. Assume it has weaknesses.
Find at least 3 specific places to improve.
If you can't find any, look harder—don't default to praise.

模板 4: 跨模型审查
───────────────────
I generated this in [Model A]: [产出]
Please critique it in [Model B] using this rubric: [rubric]

[粘贴产出 + rubric 到 Model B]
```

---

## 来自 [Recap · 模块总结](../notes/02-ai-as-thought-partner/recap.md)

### 模板 1：迭代头脑风暴

```text
I'm trying to [目标].
My context: [6 类背景].
Give me 3-5 different approaches, ranging from conservative to creative.
For each, list: main idea, trade-off, concrete example.
```

### 模板 2：Neutral + 显式要反对

```text
I'm considering [方案/论点].

Don't take my framing as truth. Present:
  - 2-3 strongest arguments FOR my position
  - 2-3 strongest arguments AGAINST
  - 1-2 alternative perspectives I might be missing
```

### 模板 3：渐进式大纲（5 步合一）

```text
Article topic: [topic]
My angle: [你的独特视角]
Counter-argument: [反对意见]
Stories: [1-2 个真实故事]

Step 1: Research 3-5 sources.
Step 2: 3 different outline options.
Step 3: I'll pick + revise.
Step 4: Expand to bullet points.
Step 5: I'll ask for prose.

Start with Step 1.
```

### 模板 4：让 AI 帮你设计 rubric

```text
I'm evaluating [essay / design / code] for [purpose].
Propose a rubric with:
  - 4-6 dimensions
  - Each dimension: 3-5 specific scoring criteria with point values
  - Total = 100 points
Make each criterion checkable (yes/no or clear pass/fail).
```

### 模板 5：跨模型审查

```text
[Model A output]
Critique using this rubric:
[rubric]
For EACH criterion, give a score AND quote the work text that
justifies it. If you can't quote anything, the score is 0.
```

---

> 返回笔记：[Module 2: AI as a Thought Partner](../notes/02-ai-as-thought-partner/README.md)
