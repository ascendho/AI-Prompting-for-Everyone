# 自测题 · Module 3: Working with Multimedia & Code

---

### Q1. 多模态 in/out 矩阵

说出 3 种**"声音输入"** + **"文字输出"** 的真实场景。

<details>
<summary>答案</summary>

1. 会议录音 → 自动转录 + 摘要
2. 播客音频 → 翻译成另一种语言
3. 客户语音留言 → 提取行动项

</details>

### Q2. 速度/成本谱排序

按"成本 + 速度"从最便宜到最贵排序：text / image / video / speech。

<details>
<summary>答案</summary>

**text < speech < image < video**

text: 秒级 + < $0.01
speech: 几秒 + < $0.05
image: 10s 秒 + 几美分
video: 分钟级 + 几十美分

</details>

### Q3. 图像理解的两个陷阱

用户问"What is in this image?"，AI 答得不完全对。哪两种情况最可能发生？

<details>
<summary>答案</summary>

1. **细粒度混淆**：两个相似物体被错认（如 [M3/02 gym machines 案例](../notes/03-working-with-multimedia-code/02-image-understanding.md)）
2. **OCR 错误**：手写字 / 模糊图被读错

**应对**：补充文字描述 + 关键信息人工核验。

</details>

### Q4. 图像生成 prompt 三要素

要把这张 prompt 改好：
> "Generate a picture of a girl."

写出包含 3 要素的版本。

<details>
<summary>答案</summary>

```
Generate an image of a girl:
  - Setting: rooftop garden in Tokyo at sunset, golden hour
  - Character details: 16-year-old, school uniform, holding a camera
  - Mood/style: cinematic, warm color palette, shot on 35mm film
```

3 要素都明确，AI 才有"足够的约束"画出你想要的图。

</details>

### Q5. Diffusion 模型的 3 大错误

分别是什么？怎么缓解？

<details>
<summary>答案</summary>

| 错误 | 缓解 |
|---|---|
| **Weird hands** | 多次生成挑选 / 用专门的 inpainting 工具修 |
| **Garbled text** | 避免在 prompt 里要 AI 写字 |
| **Inconsistent characters** | 用 reference image / 锁定详细描述 / 多生成挑选 |

</details>

### Q6. 建 app 的 3 块积木

你想做一个"提醒喝水"的 app。用 GOAL/INPUT/OUTPUT 框架写 prompt。

<details>
<summary>答案</summary>

```
GOAL: A water reminder app
INPUT: User sets their daily water goal (e.g. 8 glasses)
OUTPUT: Every 1 hour, show a notification + sound + button to log "drank 1 glass". Show progress bar.
```

3 块都明确了 → AI 才能写出有结构的代码。

</details>

### Q7. 何时用 code tool

下面哪些问题**会让 AI 自动选 code tool**？（多选）

1. "What is Python?"
2. "Show me the trend of my expenses last year"（用户上传 CSV）
3. "Tell me about photosynthesis"
4. "Which drink had the biggest sales change in my data?"（用户上传 sales.xlsx）

<details>
<summary>答案</summary>

2 和 4。

- 1 / 3 → 预训练知识（"what is"类事实）
- 2 / 4 → **数据 + 计算/画图** → 触发 code tool

</details>

---

> 返回笔记：[Module 3: Working with Multimedia & Code](../notes/03-working-with-multimedia-code/README.md)
