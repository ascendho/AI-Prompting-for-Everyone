# AI Prompting for Everyone — 学习笔记

> 我的 [AI Prompting for Everyone](https://www.deeplearning.ai/courses/ai-prompting-for-everyone)（DeepLearning.AI / Andrew Ng）课程学习笔记。
> **特点**：跳过视频看 slides + 课件，直接产出结构化笔记；配套 [prompt 模板库](../prompts/README.md) 与 [自测题](../practice/README.md)。

## 📚 课程概览

| # | 模块 | 主题 | 状态 | 笔记 |
|---|---|---|---|---|
| 1 | [01-finding-information](./01-finding-information/README.md) | Finding Information（找信息：预训练 / Web search / Deep research） | ✅ | [进入 →](./01-finding-information/README.md) |
| 2 | [02-ai-as-thought-partner](./02-ai-as-thought-partner/README.md) | AI as a Thought Partner（头脑风暴 / Context / 推理 / 拍马屁 / 写作 / 评估） | ✅ | [进入 →](./02-ai-as-thought-partner/README.md) |
| 3 | [03-working-with-multimedia-code](./03-working-with-multimedia-code/README.md) | Working with Multimedia & Code（看图 / 画图 / 建 app / 数据分析） | ✅ | [进入 →](./03-working-with-multimedia-code/README.md) |

**3 个模块全部完成。**

## 🗂 仓库结构

```
AI-Prompting-for-Everyone/
├── README.md                                    ← 仓库首页（极简入口）
├── notes/                                       ← 本目录：全部学习笔记
│   ├── README.md                                  （课程总览 + 3 模块地图）
│   ├── 01-finding-information/                    （M1 完整笔记）
│   ├── 02-ai-as-thought-partner/                  （M2 完整笔记）
│   └── 03-working-with-multimedia-code/           （M3 完整笔记）
├── prompts/                                     ← Prompt 模板库（衍生整理，非官方原文）
├── practice/                                    ← 自测题（作者自拟，非官方 Quiz）
└── slides/                                       ← 课程原始 PDF
    ├── AP4E_M1.pdf
    ├── AP4E_M2.pdf
    └── AP4E_M3.pdf
```

### 每个模块子目录内部

```
notes/01-finding-information/
├── README.md            ← M1 导读（章节地图 + 决策流程图）
├── 01-novice-vs-power-user.md   （视频 1）
├── ...                           （视频 2..N）
├── recap.md            ← 模块总结（对比表 + 决策流程图）
└── images/             ← 抽自课件的截图
```

## 🎯 我做这套笔记的初衷

- 🚫 **不刷视频**：原课视频 + 阅读 + Lab ≈ 数小时，凝练后每个模块 ~1 小时可读完。
- 🧠 **每节配套"我能马上用的 prompt 模板"**（集中在 [`prompts/`](../prompts/README.md)）：看完 → 直接复制 → 在你常用的 AI 里试。
- 📊 **大量图示 + 决策流程图**：Mermaid 流程图 + 课件原图。
- 🧪 **每章末尾的常见误区**：少踩坑。

## ✍️ 笔记风格约定

- **中文**讲解；专有名词（GPT、Deep research、Web search、Taco Bell）保留英文。
- **代码 / prompt 模板** 保留英文。
- **图示**来自课程 slides；**流程图**优先 Mermaid。
- **跨模块引用**已互链（M2 ↔ M1、M3 ↔ M1/M2）。

## 🚀 快速开始

**2 分钟看完全部 3 个模块的核心**：

1. [01-finding-information/recap.md](./01-finding-information/recap.md) — 三大工具对比
2. [02-ai-as-thought-partner/recap.md](./02-ai-as-thought-partner/recap.md) — 7 大原则
3. [03-working-with-multimedia-code/recap.md](./03-working-with-multimedia-code/recap.md) — 5 大能力

**扎实学完一个模块**：从该模块的 `README.md` 进入，按 01 → 02 → ... → recap 顺序读；配套的 prompt 模板（[`prompts/`](../prompts/README.md)）**实际跑一遍**，再做 [自测题](../practice/README.md) 检验。

## 📎 参考资料

- 课程官网：<https://www.deeplearning.ai/courses/ai-prompting-for-everyone>
- 课件 PDF：见父目录 `slides/`
- 截图原图：见各模块 `images/` 目录
