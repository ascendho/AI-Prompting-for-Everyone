# Recap: Finding Information

> **一句话核心**：AI 有 3 种「找信息」的工具——**预训练、Web search、Deep research**——你该根据问题类型挑。

## 📊 三大工具对比（课件原表）
![Finding information recap](./images/recap.png)

| | 🧠 Pretrained knowledge | 🔍 Web search | 🔬 Deep research |
|---|---|---|---|
| **例子** | Help, I dropped my phone in soup | Find me a highly rated gym nearby | Impact of daily steps on long-term health? |
| **信源数量** | 0（自给） | 几个 | 几十甚至更多 |
| **时效性** | 无关（截止前） | 最新 | 最新 |
| **AI 耗时** | 几秒 | 几十秒 | 几分钟 |
| **最适用** | 事实、定义、总结 | 实时、本地、小众 | 复杂综合 |

## 🧭 决策流程图
遇到问题时，按下面顺序问自己：

```mermaid
flowchart TD
    Q[我有一个问题] --> A{需要最新信息?<br/>新闻、趋势、当前事件}
    A -- "是" --> W[用 Web search<br/>+ 指定权威信源]
    A -- "否" --> B{涉及本地信息?<br/>我附近、我公司}
    B -- "是" --> W
    B -- "否" --> C{主题太冷门,<br/>预训练覆盖不到?}
    C -- "是" --> W
    C -- "否" --> D{问题单一具体?}
    D -- "是" --> P[用预训练知识<br/>秒答]
    D -- "否" --> E{需要跨多源综合,<br/>或需要长报告?}
    E -- "是" --> R[用 Deep research<br/>给它几分钟]
    E -- "否" --> P
    W --> F{我担心信源不可靠?}
    F -- "是" --> S[在 prompt 里显式限定<br/>WHO/官方/同行评议]
    F -- "否" --> G[直接用 AI 的搜索结果]
```

> 🎯 自测题已迁移至 [`practice/01-finding-information.md`](../../practice/01-finding-information.md)。
> 🧰 prompt 模板已迁移至 [`prompts/01-finding-information.md`](../../prompts/01-finding-information.md)。

## 🎬 Module 1 一句话总结
> **找对工具、写对 prompt。** 用预训练回答通用问题，用 web search 拿当前和本地信息（并显式指定信源），用 deep research 做需要多源综合的复杂报告。
