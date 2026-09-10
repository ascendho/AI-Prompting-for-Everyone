# 自测题 · Module 2: AI as a Thought Partner

---

### Q1. 头脑风暴配方

写出 **Brainstorming = Context + Options + Iteration** 中 **Context** 应包含哪些信息？

<details>
<summary>答案</summary>

6 类典型信息：
- 你的身份/角色/经验
- 你有的资源/约束（时间、预算、工具）
- 你不能接受的事（红线）
- 你之前尝试过/失败过的方案
- 你真正想要达成的"成功"是什么
- 你的隐藏 context（trampoline、cat 之类）

</details>

### Q2. Context 的"陷阱"

下面哪些是"相关 context"，哪些是"不相关 context"？

1. 你给 AI 看 100 页租赁合同，让它帮你做 tradeoffs 决策
2. 你让 AI 帮你写妈妈健身计划，但 chat history 里全是你自己的偏好
3. 你让 AI 写代码，附上项目的 README 和 design doc
4. 你让 AI 写新功能，但 chat history 是上个月给完全另一个项目的调试

<details>
<summary>答案</summary>

1. ✅ **相关** — 决策需要看完整文档
2. ❌ **不相关** — 你的偏好不能套到妈妈身上（应开新对话）
3. ✅ **相关** — 代码生成需要项目上下文
4. ❌ **不相关** — 应该开新对话

</details>

### Q3. Desktop app 安全

你让 Claude Cowork 整理你 ~/Documents/research 目录。它提出"删除 47 个看起来过时的文件"。你应该怎么做？

<details>
<summary>答案</summary>

1. **先备份**整个目录（或至少备份待删除文件）—— 删除不进回收站。
2. **审查清单**：它怎么判断"过时"？是否会误删你需要的？
3. **缩窄权限**：让它先只**重命名**到 _to_delete/ 子目录，确认无误后再删。
4. **拒绝任何"permanently delete"权限**除非你真的需要。

</details>

### Q4. Reasoning 4 铁律

「Write me a comprehensive 12-month plan for a 4-person AI startup with limited cash」这个 prompt 缺什么？

<details>
<summary>答案</summary>

按 4 铁律诊断：
- **最好模型** — 默认用什么？应该用 Opus 4.6 / GPT 5.2。
- **够 context** — 没给"limited cash" 具体数字、没给团队技能、没给产品方向。
- **难任务** — "comprehensive" 太模糊；应该具体到"month 1, 2, 3..." 的里程碑。
- **think hard** — 没说要 "think / ultrathink"。

**改进版**：

```
I'm designing a 12-month plan for a 4-person AI startup.
Context:
  - Founders: 2 engineers, 1 PM, 1 designer
  - Cash: $500K
  - Product: developer tools (AI code review)
  - Goal: 100 paying teams by month 12
Use the best reasoning model. Think hard. Output: month-by-month
milestones, hiring plan, cash burn, key risks, decision points.
```

</details>

### Q5. Sycophancy 识别

判断下面哪些是 sycophancy：

1. 用户：「What do you think of my startup idea?」AI：「This is a fantastic idea! Very creative!」
2. 用户：「Find all the positive metrics in this data」AI：「Revenue growth, retention improving, margins up.」
3. 用户：「Is this essay any good?」AI：「Let me give you 3 specific places to improve: …」

<details>
<summary>答案</summary>

1. ✅ **是 sycophancy** — 没用 rubric，没具体，全是夸。
2. ⚠️ **可能是隐蔽 sycophancy** — 用户限定"positive"，AI 就**只挑 positive**。**真正的客观分析应该包括 negative**。这里要看：用户在第 1 步就已经限定了"只报 positive"——**问题在 prompt 而非 AI**，但 AI 没有主动指出"你这样问会引导我选择性呈现"。
3. ❌ **不是 sycophancy** — 给了 3 个具体改进点。即使开头有些礼貌，也不算讨好。

</details>

### Q6. AI 写作指纹

下面这段话里挑出 AI 写作指纹：

"Delving into the nuanced landscape of remote work, it's clear that this isn't just about flexibility—it's about autonomy, productivity, and well-being. Our robust research reveals a compelling picture of how distributed teams can thrive."

<details>
<summary>答案</summary>

- **"Delve"** — 过度使用
- **"nuanced"** — 过度使用
- **"robust"** — 过度使用
- **"compelling"** — 过度使用
- **"not just X—it's about A, B, and C"** — "not x but y" 句式
- **"clear that"** — 模糊空话
- **em dash** — 过度使用

整段都是 AI fingerprint。建议改写：

"Remote work changes three things: flexibility, autonomy, and how teams measure productivity. Our [data source] shows [specific finding]."

</details>

### Q7. Rubric 评估

下面两个 rubric 哪个更好？为什么？

**A**：「Characters (25 points), Plot (25 points), World building (25 points), Writing craft (25 points)」

**B**：「Characters (25 points):
- Every named character has a goal (10 points)
- Conflict between two characters' goals (10 points)
- At least one character makes an irreversible decision (5 points)」
（Plot / World building / Writing craft 类似展开）

<details>
<summary>答案</summary>

**B 更好**。原因：
- **每个维度有具体评分点** → AI 必须逐项打勾，没法用"great!"糊弄。
- A 的 "Characters 25 points" 让 AI 凭感觉给分 → **容易给 20+ 分** → 整体偏高 → sycophancy 漏洞。
- B 让评分**可重复**——同一个人用同一份 rubric 给同一篇文打分，结果应该接近。

</details>

---

> 返回笔记：[Module 2: AI as a Thought Partner](../notes/02-ai-as-thought-partner/README.md)
