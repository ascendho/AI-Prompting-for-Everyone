# Prompt 模板 · Module 3: Working with Multimedia & Code

---

## 来自 [01. Working with multimedia data](../notes/03-working-with-multimedia-code/01-multimedia-overview.md)

```text
模板 1: 多模态创意（图像参考 + 文字 prompt）
───────────────────
[上传参考图]
Based on this image's style/character, generate 3 new ideas
for [你的目标]. For each, describe the image you'd want to generate.

模板 2: 多模态输入（图片+声音+文字）
───────────────────
[上传图片]
[上传声音文件，如果支持]
[文字 prompt]
Combine all inputs to [目标]. Reference specific elements from each.

模板 3: 控制成本的多模态 prompt
───────────────────
I'm on a budget. Before generating, propose a single
best [image/video/audio] concept with:
  - A clear description
  - The exact prompt I should use
  - The size/duration/style to minimize cost

Generate ONLY after I approve.

模板 4: 负责任使用
───────────────────
[生成内容前]
Will this content be used to:
  - Represent a real person (yes/no)?
  - Deceive viewers (yes/no)?
If yes to either, add a clear disclosure/watermark.
```

---

## 来自 [02. Image understanding](../notes/03-working-with-multimedia-code/02-image-understanding.md)

```text
模板 1: 单图 + 文字提问
───────────────────
[上传图片]
What is this? Be specific. If you can't tell, say so.

模板 2: 多图 + 总结
───────────────────
[上传多张图片 + 关联的 notes.docx]
Summarize the meeting. Identify:
  - Main topics discussed
  - Decisions made
  - Open questions
  - Action items + owners

模板 3: 细粒度识别（防 AI 混淆）
───────────────────
[上传图片]
These two objects LOOK similar but are different.
Focus on [specific feature: 把手位置 / 颜色 / 形状 / 文字标签].
Tell me which is which, with a 1-sentence reason.

模板 4: OCR + 推理
───────────────────
[上传账单 / 表格 / 文档照片]
Extract all text. Then answer: [你的具体问题，比如"我点了几样、多少钱"]

模板 5: 视觉不靠谱时的兜底
───────────────────
I tried OCR on this and AI mis-identified it.
Here's what I think it is: [你的猜测].
Confirm or correct, and explain your reasoning.
```

---

## 来自 [03. Image generation](../notes/03-working-with-multimedia-code/03-image-generation.md)

```text
模板 1: 三要素结构化 prompt
───────────────────
Generate an image with:
  - Setting: [场景、时间、天气、室内/外]
  - Character: [主体描述，外貌、穿着、动作]
  - Mood/style: [艺术风格 + 情绪]

Example: Generate an image of a cat secretly running a coffee shop.
  - Setting: nighttime cozy café interior
  - Character: clever orange tabby cat, tiny apron, standing on stool
  - Mood/style: whimsical, cartoon style, warm lighting

模板 2: 风格切换
───────────────────
Generate the same image in 4 styles:
  1. Cinematic
  2. Watercolor
  3. Cyberpunk neon
  4. Studio Ghibli anime

I'll pick one and refine.

模板 3: 编辑现有图
───────────────────
[上传图片]
Edit this image to:
  - Remove: [反光 / 路人 / 文字 / 杂物]
  - Add: [新元素]
  - Change: [颜色 / 背景 / 比例]
Keep everything else identical.

模板 4: 角色一致性
───────────────────
[上传角色的 reference 图]
Maintain this exact character's appearance (face, body type, color,
clothing) across all 4 panels of a comic strip:
  Panel 1: [action]
  Panel 2: [action]
  Panel 3: [action]
  Panel 4: [action]

模板 5: 控制成本
───────────────────
Before generating, describe the image you would create in detail.
I'll review and either approve or revise BEFORE you spend generation
budget. Only generate after I say "go".
```

---

## 来自 [04. Building apps](../notes/03-working-with-multimedia-code/04-building-apps.md)

```text
模板 1: 标准 app prompt
───────────────────
GOAL: [这个 app 解决什么问题 / 提供什么体验]
INPUT: [用户怎么用 — 按钮、文本、点击、滑动]
OUTPUT: [app 怎么响应 — 显示什么、计算什么、生成什么]

例子:
GOAL: A pomodoro timer for focused work
INPUT: Click Start to begin 25 min; see remaining time
OUTPUT: Countdown, sound when done, switch to break mode

模板 2: 实用工具
───────────────────
GOAL: A bill calculator for splitting restaurant bills
INPUT: Total bill amount + number of people + tip %
OUTPUT: Per-person amount, including tax and tip

模板 3: 探索 3 个版本
───────────────────
[App idea]

Propose 3 versions with different complexity:
  V1: Minimum viable (single user, local data)
  V2: Mid-tier (some persistence, basic UI)
  V3: Full-featured (multi-user, AI integration)

I'll pick one.

模板 4: 迭代改进
───────────────────
[粘贴现有 app 代码 / 描述]
Things to add:
  - [功能 A]
  - [功能 B]

Refactor the code. Keep the same tech stack. Add unit tests
for the new features.
```

---

## 来自 [05. Data analysis](../notes/03-working-with-multimedia-code/05-data-analysis.md)

```text
模板 1: 上传数据 + 自由探索
───────────────────
[上传 CSV / Excel]
Analyze this data. Tell me:
  - Key trends (increasing / decreasing / stable)
  - Any anomalies or outliers
  - 1-3 actionable recommendations

模板 2: 明确的分析任务
───────────────────
[上传数据]
Calculate [metric] by [dimension]. Show me:
  - A summary table
  - A chart
  - 1-2 sentences interpretation

例子: Calculate monthly revenue by product. Show me
a table, a chart, and explain what's driving the changes.

模板 3: 多轮迭代（M2 的迭代原则）
───────────────────
[上传数据]
Round 1: Show me the top 5 most important findings.
[看到结果后]
Round 2: For the most interesting finding, dig deeper.
What are the contributing factors? Show me a breakdown.
[继续]
Round 3: Based on this, suggest 3 specific actions I can take.

模板 4: 强制 code tool
───────────────────
[上传数据]
Use the code tool to:
  - Load the data
  - Compute [specific calculation]
  - Generate a visualization
Show me the code you used and explain each step.
```

---

## 来自 [Recap · 模块总结](../notes/03-working-with-multimedia-code/recap.md)

### 模板 1：图像理解 + 文字 prompt

```text
[上传图片]
What is this? If you see text, transcribe it.
For the main subject: describe its appearance, position, and any
text/numbers visible. If you can't tell, say "I can't tell".
```

### 模板 2：图像生成三要素

```text
Generate an image with:
  - Setting: [场景]
  - Character: [主体 + 外貌 + 动作]
  - Mood/style: [艺术风格] + [情绪]
```

### 模板 3：编辑图片

```text
[上传图片]
Edit this image to:
  - Remove: [...]
  - Add: [...]
  - Change: [...]
Keep everything else identical. Maintain the same style.
```

### 模板 4：建 app

```text
GOAL: [...]
INPUT: [...]
OUTPUT: [...]

Tech stack: [HTML+JS / Python+Flask / etc.]
Keep it minimal. Include a README with how to run.
```

### 模板 5：分析数据

```text
[上传 CSV/Excel]
Use the code tool to:
  1. Load and inspect the data
  2. Compute [specific calculation]
  3. Generate a visualization
  4. Tell me 1-3 actionable insights

Show me the code you wrote.
```

---

> 返回笔记：[Module 3: Working with Multimedia & Code](../notes/03-working-with-multimedia-code/README.md)
