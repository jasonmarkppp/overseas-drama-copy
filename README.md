# Overseas Drama Copy

面向英文婚姻背叛短剧推广文案的 Codex Skill：保持客户参考的高情绪强度，输出英文正文、中文对照和双语标题，并检查剧情因果、英文自然度、翻译与历史重复。

## 状态

v0.1 候选版。文件结构已校验；仍需客户跨场景验收。没有真实投放结果，不保证爆款，也不将模型自审等同于母语人工审稿。

## 安装

将整个仓库放入 Codex skills 目录，确保结构为 `overseas-drama-copy/SKILL.md`。私有仓库需要相应 GitHub 访问权限。

Windows PowerShell（目标目录尚不存在时）：

```powershell
git clone https://github.com/jasonmarkppp/overseas-drama-copy.git "$env:USERPROFILE\.codex\skills\overseas-drama-copy"
```

如果该目录已有版本，在原目录更新或保留备份，不需要重复克隆。

## 使用

```text
使用 $overseas-drama-copy 生成一篇新的原创案例。
保持参考文案的情绪强度，提供英文标题、中文标题、英文正文、中文对照。
交付前检查英文、剧情因果和翻译，不重复已有案例的事件链。
```

已有原剧时一并提供剧情资料；Skill 不会把自行编造的事件冒充原剧情。需要连续测试时，将作品和真实反馈保存在当前项目的 `drama-copy-lab` 目录。

## 文件

- `SKILL.md`：生成、审核及反馈更新流程。
- `references/client-style.md`：客户风格证据、已知失败与反馈边界。
- `agents/openai.yaml`：Codex 中的名称与默认调用提示。

本仓库不包含客户原始参考附件或项目测试稿。流程无需外部 API、网页或向量数据库。
