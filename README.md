# AI Learning Companion

一个基于真实学习资料工作的 AI 陪伴学习 Skill。

它不会在收到任务后立刻生成答案，而是先确认学习领域、目标、基础、知识卡点和资料可访问状态，再通过用户确认的“学习任务卡”进入执行。

支持三个可以独立使用或依次执行的模块：

1. **知识地图**：把大体量或零散资料整理为可回到原文核对的结构稿；在宿主 Agent 具备图片生成能力时，还可以进一步生成可视化总图。
2. **通用场景类比**：把相近、抽象概念放进同一个生活场景中比较。
3. **费曼检验**：让学习者先解释，再通过连续追问暴露理解漏洞。

## 适用范围与能力边界

这个仓库提供的是一套 **Agent Skill 指令与工作流**，不包含大模型、图片生成模型、OCR、PDF 解析器或文件存储服务。实际效果取决于安装它的 Agent、模型和可用工具。

### 平台兼容性

- **Codex**：可以通过 `$skill-installer` 安装并使用，是当前主要验证环境。
- **兼容 `SKILL.md + references/` 结构的 Agent**：通常可以直接安装或手动复制技能目录；`agents/openai.yaml` 不受支持时可以忽略。
- **普通 ChatGPT、Claude 网页版或没有 Skill 机制的平台**：不能保证通过 GitHub 地址一键安装。可以手动上传 `SKILL.md` 和 `references/three-stage-workflow.md`，但是否能稳定遵循完整流程取决于模型能力和平台上下文限制。

### 知识地图的输出能力

- 仅具备文本能力的模型，可以完成资料索引、可核对的 Markdown 结构稿，以及供其他制图工具使用的视觉规格。
- 只有宿主 Agent 同时具备可调用的**图片生成工具或图像生成能力**时，才能直接生成最终知识地图图片。能识别图片的“多模态模型”不一定也能生成图片。
- 如果图片生成不可用，Skill 会退回结构化视觉稿，不会声称已经产出图片。

### 资料访问与结果可靠性

- Agent 必须确实能够访问用户上传的资料。只给出它无法访问的本地路径时，Skill 会要求上传文件或粘贴必要内容。
- Skill 要求保留来源定位，并标记“资料外补充”和“待核对”；但输出准确性仍受源资料质量、模型推理能力和上下文容量影响。
- 费曼评分只用于暴露理解漏洞，不是考试成绩、能力认证或客观结论。

## 安装

在 Codex 中调用 `$skill-installer`，并提供以下 GitHub 路径：

```text
https://github.com/linnanwu111-dev/ai-learning-companion/tree/main/ai-learning-companion
```

也可以手动安装：

```bash
git clone https://github.com/linnanwu111-dev/ai-learning-companion.git
cp -R ai-learning-companion/ai-learning-companion ~/.codex/skills/
```

## 使用

```text
使用 $ai-learning-companion，根据我提供的资料陪我学习一个复杂主题。
```

Skill 会先收集必要信息并输出学习任务卡；确认前不会直接开始生成知识地图、类比或测试题。

## 目录

```text
ai-learning-companion/
├── SKILL.md
├── agents/openai.yaml
└── references/three-stage-workflow.md
```

## License

MIT
