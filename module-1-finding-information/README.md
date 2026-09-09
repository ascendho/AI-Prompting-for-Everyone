# Module 1: Finding Information

> **本模块核心**：知道 AI 模型「怎么找到信息」以及「什么时候该让它去找」，是写出好 prompt 的基础。

## 🎯 学习目标

学完这一模块，你应该能：

1. 区分 **AI novice** 和 **AI power user** 的行为差异，并把 5 个对比场景套用到自己的 prompt 改写中。
2. 理解 **pretrained knowledge**（预训练知识）的来源、边界和限制。
3. 知道何时该用 **web search**，以及怎么显式触发。
4. 知道 web search 拉到的信息未必可靠，掌握 **引导权威信源** 的 prompt 技巧。
5. 理解 **deep research**（深度研究）跟普通 web search 的差异，知道什么时候值得花时间等它。

## 🗂 章节地图

| 章节 | 标题 | 对应课件 | 阅读时间 |
|---|---|---|---|
| [01](./01-novice-vs-power-user.md) | The AI novice and the AI power user | 视频 1 (9m) | ~12 min |
| [02](./02-pretrained-knowledge.md) | Pretrained knowledge | 视频 2 (6m) | ~10 min |
| [03](./03-web-search.md) | Web search | 视频 3 (5m) | ~8 min |
| [04](./04-web-search-sources.md) | Web search sources | 视频 4 (8m) | ~12 min |
| [05](./05-deep-research.md) | Using deep research | 视频 5 (8m) | ~12 min |
| [06](./06-lab-overview.md) | Lab overview: AI model prompt comparison | 视频 6 (4m) + Lab | ~15 min |
| [recap](./recap.md) | Finding information 总览 + 三大工具对比 | Recap | ~10 min |

**建议**：按顺序看，每节末尾的「🛠 我能马上用的 prompt 模板」可以一边看一边在自己常用的 AI 里试一下，再去 [Module 1 Quiz](https://www.deeplearning.ai/courses/ai-prompting-for-everyone) 检验。

## 📐 模块主线

```
        你有一个问题
              │
              ▼
   ┌──────────────────────┐
   │  预训练知识够用吗？    │
   └──────────┬───────────┘
              │ 不够
              ▼
   ┌──────────────────────┐
   │  需要实时/本地/小众？  │ ── 是 ──▶  Web search
   └──────────┬───────────┘                │
              │ 否                          ▼
              ▼                     想要权威来源？
   ┌──────────────────────┐          │
   │  复杂综合 / 多子题？  │          ▼
   └──────────┬───────────┘     显式指明信源
              │ 是
              ▼
        Deep research
```

详细决策流程见 [recap.md](./recap.md)。

## 📎 资源

- 课程官网：<https://www.deeplearning.ai/courses/ai-prompting-for-everyone>
- 课件 PDF：见父目录 `slides/AP4E_M1.pdf`（仅 M1 入仓；M2/M3 待学完后补）
- 图片来源：所有 `images/` 下截图均抽自上述课件
