# careKind AI — 公司规范

版本 v1.0；生效日期 2026 年 10 月 4 日。适用于团队成员及执行公司任务的 Claude/Codex。

| 规范 | 使用范围 |
|---|---|
| [公司规范](company.md) | 公司职责、决策、资料管理和协作 |
| [运营规范](operations.md) | 客户、市场宣传、试点、HR 与运营记录 |
| [产品与法律参考规范](product-and-legal.md) | 产品设计、PRD、功能/数据流变更及法律依据 |
| [代码规范](coding.md) | SOLID、DRY、KISS；Tab 宽度 4；16 条执行规则，单个代码文件超过 1,000 行自动重构 |
| [分层文档规范](documentation.md) | 根目录、部门与大型功能模块的 AGENTS.md、CLAUDE.md 和 README.md 职责及维护 |
| [AI 修改记录规范](changelog.md) | 每次 AI 修改追加到根目录 CHANGELOG.md，保留原因、文件、执行者和检查结果 |

类型例外采用 [any / Any 白名单](any-whitelist.md)，当前没有批准项。本地秘密文件由项目 `.gitignore` 排除，代码缩进由 `.editorconfig` 定义。

公司规范作为共同基础；按任务读取对应专项规范。产品设计或新建/修订 PRD 必须执行产品与法律参考规范，编码必须执行代码规范。项目 AGENTS.md 与 CLAUDE.md 引用本目录；技能与工作流继续描述具体执行步骤。

共用 PRD 在 `docs/PRD_careKind_AI.md`，现有合规责任和试点准入文件在 `Marketing & Operations/Company OS/`。本目录定义工作标准，不复制法律全文或替代已有专项政策。发现规范、需求和实际证据矛盾时，记录冲突与待决定事项，不静默改写依据。

规范修订记录原因、日期、受影响文件和决策状态。仅需根据当前任务做对应检查；无需因小型文档修改执行完整上线流程。
