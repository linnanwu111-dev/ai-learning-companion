# AI Learning Companion

一个基于真实学习资料工作的 AI 陪伴学习 Skill。

它不会在收到任务后立刻生成答案，而是先确认学习领域、目标、基础、知识卡点和资料可访问状态，再通过用户确认的“学习任务卡”进入执行。

支持三个可以独立使用或依次执行的模块：

1. **知识地图**：把大体量或零散资料整理为可回到原文核对的知识结构。
2. **通用场景类比**：把相近、抽象概念放进同一个生活场景中比较。
3. **费曼检验**：让学习者先解释，再通过连续追问暴露理解漏洞。

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
