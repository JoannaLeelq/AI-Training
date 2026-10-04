# 工作流 — Workflows

共用流程供 Claude Code 和 Codex 在收到任务后选择并执行。流程定义输入、步骤、输出和完成条件；`../skills/` 保存对应的标准 SKILL.md。

| 工作流 | 输入 | 输出位置 |
|---|---|---|
| [产品开发](product-delivery.md) | 产品目标、需求、bug 或开发任务 | 产品需求 `docs/`；技术实现 `APP Development/` |
| [市场与竞品研究](market-research.md) | 调研问题、市场/供应商范围 | `Marketing & Operations/Research/` |
| [法规与文书研究](compliance-research.md) | 产品功能、州/领地、服务类型 | `Marketing & Operations/Research/` |
| [公司与团队运营](operations.md) | OS、人员角色、运营或营销任务 | `Marketing & Operations/` 或 `HR & Teams/` |
| [反馈分析](feedback-analysis.md) | Joanna 明确要求分析的原始反馈 | `Feedback/analysis/` |

## 使用方法

建议将 `careKind AI` 作为项目文件夹打开或从此目录启动工具。两个工具的本地入口技能叫 `carekind-workflow`：Codex 可以用 `$carekind-workflow`，Claude Code 可以用 `/carekind-workflow`。也可以直接用自然语言交办，例如“按工作流准备一个护理记录草稿功能的需求文档”。匹配技能可以由工具自行选择。

从上一级 `AI Training` 启动时，根目录的 AGENTS.md / CLAUDE.md 将任务引导至公司的共用说明；若本地技能菜单未显示，进入 `careKind AI` 后新开会话，或直接要求读取对应 SKILL.md。

当前配置用于**任务触发后的自动执行**。文件本身不会定时启动 Claude/Codex，也不替代工具权限、项目可信设置、登录或外部服务凭证。未配置无人值守调度。

多步骤任务使用 [执行记录模板](run-record-template.md)。状态为进行中、阻塞或完成；完成需要交付物和实际检查结果。raw 反馈没有 AI 录入工作流。

## 入口依据

- [Codex 技能及发现路径](https://learn.chatgpt.com/docs/build-skills)
- [Codex AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
- [Claude Code CLAUDE.md 和共享说明导入](https://code.claude.com/docs/en/memory)
