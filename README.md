# 互动式论文导读 · Paper Reading Tutor

`paper-reading-tutor` 是一个陪你分轮读技术论文的 Codex 技能。它会先了解你的阅读目标和基础，再用原文图表、小例子和手算讲清关键方法。每轮通常留一道小题，根据你的回答决定补讲哪里、什么时候继续。

适合刚开始读 AI、计算机或工程论文的学生，也适合换到陌生领域时从基础读起。可以陪你通读整篇，也可以只讲某个方法、公式或实验结果。

## 安装

在 Codex 对话里发送这条消息。

```text
$skill-installer 请从 https://github.com/luteyinuo/paper-reading-tutor/tree/main/paper-reading-tutor 安装 paper-reading-tutor 技能。
```

手动安装时，在 GitHub 下载并解压仓库 ZIP，再把 `paper-reading-tutor/` 整个目录复制到个人技能目录 `~/.agents/skills/` 下（Windows 为 `%USERPROFILE%\.agents\skills\`）。如果技能未显示，试着重启 Codex。[Codex 技能官方文档](https://learn.chatgpt.com/docs/build-skills)

## 开始导读

把论文 PDF 提供给 Codex，或告诉它论文在当前工作区中的位置，然后发送这条消息。

```text
$paper-reading-tutor 陪我分轮读懂这篇论文。我是初学者，请先问我的阅读目标和基础。讲到图表时请对照原图，遇到关键公式请用一组小数字手算。
```

也可以指定「只讲方法」「跳过练习」「这节一次讲完」，或说明你要准备一场 15 分钟的组会汇报。

## 导读流程

通读时，技能会逐张讲解主文图表，用小例子解释主要公式，最后请你用自己的话串起研究问题、方法、证据和局限。准备汇报或代码复现时，可以沿用已经读懂的内容继续做。

## 仓库结构

- [`paper-reading-tutor/SKILL.md`](paper-reading-tutor/SKILL.md) — 导读流程、讲解方式和续讲规则。
- [`paper-reading-tutor/agents/openai.yaml`](paper-reading-tutor/agents/openai.yaml) — 技能在 Codex 中的显示信息。
