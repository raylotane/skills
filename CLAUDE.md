# Skills 仓库

这是一个 Claude Code skills 的开发和存储仓库。每个 skill 是一个独立目录，包含 `SKILL.md` 和可选的 `references/`、`scripts/`、`assets/`。

## Skill 结构

```
skill-name/
├── SKILL.md        # 必须：skill 定义（YAML frontmatter + markdown 指令）
├── references/     # 按需加载的参考文件
├── scripts/        # 可执行脚本
└── assets/         # 模板、图标等资源
```

## 已有 Skill

- `musk-brain` — 马斯克式思维路由器，分析用户场景后路由到对应思维框架
- `project-pulse` — 项目脉搏分析，综合上下文后给出行动建议

## 开发 Skill 时

- 使用 `/skill-creator` 命令进入 skill 创建流程
- SKILL.md frontmatter 的 `description` 是关键，它决定 skill 何时被触发
- description 要写清楚触发条件和使用场景，宁可偏"pushy"也不要被漏触发
- 遵循 skill-creator 的 test → review → improve 循环
