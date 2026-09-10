# Prompt 模板 · Module 1: Finding Information

---

## 来自 [01. The AI novice and the AI power user](../notes/01-finding-information/01-novice-vs-power-user.md)

```text
模板 1: 问难的问题
───────────────────
[把上下文文件粘贴进来]
Compare these [N] options across [维度 1, 维度 2, 维度 3].
Think hard before answering. Show me a comparison table.

模板 2: 自评 / 写作类
───────────────────
[粘贴过去的工作记录、笔记、链接]
Write a self-review based on what I actually did. Avoid generic phrases
like "I'm a hard worker" or "I go above and beyond".

模板 3: 要诚实反馈
───────────────────
[把你的方案 / 想法 描述清楚]
Critique the following idea objectively. Use this rubric:
  - Problem & market (0-20)
  - Solution & value prop (0-20)
  - Competitive advantage (0-20)
  - Business model (0-20)
  - Feasibility & execution (0-20)
Be specific. Don't hedge.

模板 4: 写作协作（不要一步到位）
───────────────────
Step 1: Outline a blog post about [topic] based on these notes:
        [粘贴 notes.txt]
Step 2: (review outline) Skip section [X]. Add an anecdote about [Y].
Step 3: Expand the revised outline into bullet points.
Step 4: Turn the bullets into prose.
```

---

## 来自 [02. Pretrained knowledge](../notes/01-finding-information/02-pretrained-knowledge.md)

```text
模板 1: 显式让 AI 用「它的内置知识」回答
───────────────────
Using only your pretrained knowledge (no web search), explain [topic].

适用：你想测一下 AI 自身理解到什么程度（不受搜索结果影响）。

模板 2: 让 AI 标注「哪段来自预训练、哪段不确定」
───────────────────
Answer this question. For each claim, mark confidence as
[high / medium / low] based on how well-represented it is in your
training data. Flag anything time-sensitive as low.

适用：你想知道 AI 哪些回答值得信、哪些要去二次查证。

模板 3: 让 AI 提醒「训练截止」带来的局限
───────────────────
What is your knowledge cutoff date? Then answer [question],
and clearly separate what you know vs. what might have changed since.
```

---

## 来自 [03. Web search](../notes/01-finding-information/03-web-search.md)

```text
模板 1: 显式要求 web search 并标注来源
───────────────────
Search the web for [question]. Provide a synthesized answer with
inline citations (link + source name). If sources disagree, say so.

模板 2: 强制时间过滤
───────────────────
Search the web for [topic]. Only consider sources from the past
[3 / 6 / 12] months. Ignore older articles unless they're the only
authoritative source.

模板 3: 强制地域过滤
───────────────────
Find me [商品/服务/地点] in [城市, 国家]. Use local business
directories and recent reviews. Show me a ranked list with
ratings and last-review date.

模板 4: 小众话题的深挖
───────────────────
Search the web for [niche term]. I want to know:
  - the canonical definition
  - the top 3 most-cited sources
  - any controversies or competing views
```

---

## 来自 [04. Web search sources](../notes/01-finding-information/04-web-search-sources.md)

```text
模板 1: 显式指定信源等级
───────────────────
Search the web for [topic]. Prioritize:
  1. Official government / institutional sources
  2. Peer-reviewed research
  3. Established news outlets
Avoid: blogspam, SEO content farms, social media posts.

模板 2: 排除过时信息
───────────────────
Search the web for [topic]. Only include sources from the last
[6 months / 1 year]. Explicitly flag any results that look
stale or whose publish date is older than your cutoff.

模板 3: 要求显示信源
───────────────────
Search the web and present the answer as a bullet list.
For each bullet, show:
  - The claim
  - The source (name + URL)
  - The publication date
  - A 1-sentence reason this source is credible

模板 4: 跨源对比
───────────────────
Search the web for [controversial topic]. Find at least 3 sources
with different viewpoints. Present a comparison table:
Source | Position | Key argument | Date | Credibility (1-5).
```

---

## 来自 [05. Using deep research](../notes/01-finding-information/05-deep-research.md)

```text
模板 1: 触发 deep research
───────────────────
Do a deep research on [topic]. Before answering, plan the
sub-questions you'll investigate. Iterate on your searches
until you have authoritative sources. Deliver a report
with inline citations.

模板 2: 限定 deep research 的边界
───────────────────
Deep research [topic] with these constraints:
  - Geographic focus: [国家/城市]
  - Time range: last [N] years
  - Source priority: peer-reviewed > government > reputable media
  - Length: 1500-2000 words
  - Output: report with sections + citations

模板 3: 让 deep research 给出可执行建议
───────────────────
Deep research [problem]. I need not just facts, but a concrete
action plan I can start this week. Include:
  - Background (the relevant context)
  - Key findings
  - Risks
  - Step-by-step action plan
  - Open questions to investigate further
```

---

## 来自 [Recap · 模块总结](../notes/01-finding-information/recap.md)

### 模板 1：限定权威信源

```text
Search the web for [topic]. Prioritize:
  1. Official government / institutional sources
  2. Peer-reviewed research
  3. Established news outlets
Avoid: blogspam, SEO content farms, social media.
```

### 模板 2：要求带引用的综合

```text
Search the web and synthesize an answer. For each key claim,
provide an inline citation (URL + source name + date).
If sources disagree, list the disagreements explicitly.
```

### 模板 3：深度研究的边界

```text
Do a deep research on [topic]. Constraints:
  - Geographic focus: [国家/城市]
  - Time range: last [N] years
  - Length: 1500-2000 words
  - Output: report with sections + inline citations
```

### 模板 4：批判性反馈

```text
Critique the following idea objectively. Use this rubric:
  - Problem & market (0-20)
  - Solution & value prop (0-20)
  - Competitive advantage (0-20)
  - Business model (0-20)
  - Feasibility & execution (0-20)
Be specific. Don't hedge.
```

### 模板 5：写作协作 outline → expand

```text
Step 1: Outline a blog post about [topic] based on these notes:
        [paste notes]
Step 2: Skip section [X]. Add an anecdote about [Y].
Step 3: Expand the revised outline into bullet points.
Step 4: Turn bullets into prose.
```

---

> 返回笔记：[Module 1: Finding Information](../notes/01-finding-information/README.md)
