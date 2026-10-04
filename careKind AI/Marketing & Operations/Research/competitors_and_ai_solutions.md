# careKind AI：澳洲 aged care 竞争者与 AI 文书产品扫描

**研究日期：** 2026 年 10 月 4 日  
**范围：** 面向澳洲 residential aged care 与 home/community care 的临床文书、护理记录和相邻 AI 产品。公开网站资料用于初筛，不等于独立产品验证；供应商的性能、合规和客户成效声明均需尽调。

## 市场概况

澳洲 aged care 已有一批成熟的 care/clinical management system（CMS）作为日常记录系统。Services Australia 的公开 online-claiming 软件名单列出 Acredia Care、AlayaCare、Leecare、Telstra Health 等供应商，覆盖 residential care、Support at Home 或两者。它不是完整市场份额榜单，也不代表政府推荐。 [Services Australia：aged care 软件名单](https://www.servicesaustralia.gov.au/software-for-aged-care-online-claiming?context=20)

新 AI 竞争者主要走三条路线：① 在现有 CMS 外围把语音/文字转成记录草稿；② 直接把 AI 嵌入完整 care platform；③ 读取既有记录，做摘要、质量提示和风险线索。成熟 CMS 的整合和工作流优势很强；单点 AI 的胜负关键将是护士是否愿意在真实班次中使用、能否写入现有系统，以及能否证明记录忠实、可追溯且经人审核。

## 主要竞争者

| 供应商 / 产品 | 目标与定位 | 公开披露的文书 / AI 能力 | 差异点与注意事项 |
|---|---|---|---|
| **MediQo – Aged Care Documentation** | 专为 aged care 护理互动记录，面向 residential aged care | 声称可聆听照护互动并生成 progress notes、shift handovers、临时 care plans、incident reports、food/fluid records；工作人员审核、修改、批准后才加入 resident record；支持 140 多种语言的安全语音 dictation。 [产品说明](https://www.mediqo.health/solutions/aged-care-documentation) | 与 care interaction 的现场语音流程直接竞争。公开页面没有说明与哪些澳洲 CMS 已实际集成、部署规模、定价或独立验证结果，需销售验证。 |
| **Notive** | 早期澳洲 aged care 语音 shift-note 工具，页面称目前在南澳招募少量 founding facilities | 口述后生成 handover note，员工 review/edit/finalise；宣称单名 resident 90 秒内完成；声称澳洲 Sydney 存储、转录后立即删除音频、按角色授权及永久审计日志。 [产品页](https://notive.com.au/) | 与 careKind 的 nurse/carer note drafting 最直接。公开页提供 7 日试用，后续按机构规模议价；暂无公开价目。该页自述的“compliant”“tamper-proof”等应当作供应商声明，不是独立审计结论。 |
| **AgedCareAI – Suite** | 面向 residential、home care package、community providers 的 aged-care 专用 AI 套件 | 公开模块包括 Assist（在既有系统中改进 notes/reports、填表、问答）、Canvas（实时写作）、Forms、Whisper、AskMe（政策/程序/标准问答）、360View 和 analytics/workflows。 [产品套件](https://www.agedcareai.com.au/suite) | 覆盖面较广、强调在现有软件旁工作和机构数据治理；不仅是语音转记录。需要核实各模块当前可售/上线状态、具体集成、模型与数据流、客户实例。公开资料未列价格。 |
| **Acredia Intelligence** | 澳大利亚 residential aged care 临床管理平台的内嵌 AI add-on | 读取团队已有文档，生成 shift summaries、resident history，找出相似记录，并检查 incident 文档完整度；称输出有来源、可审阅和留痕，AI 不做临床判断；供应商称数据在 AWS Sydney/Melbourne、自建处理设施。 [AI add-on](https://acredia.au/intelligence/)；[平台方案](https://acredia.au/solutions/) | 核心差异是已有 aged-care clinical platform、源记录上下文及一体化 workflow；不是主要以“听现场对话写记录”为卖点。其在澳洲托管和无第三方 AI 访问均为供应商公开声明，仍要索取合同、架构及审计证据。 |
| **AlayaCare – AI Form Assistant / Layla / AlayaFlow** | 大型 home/community care 平台，并提供 residential 产品；目标覆盖 care operations | 澳洲站称 AI Form Assistant 将语音转成表单字段，Layla 提供平台内问答/摘要，AI Smart Summaries 汇总客户、员工、forms 和 progress notes；AlayaFlow 宣传 intake、scheduling、clinical agents。 [澳洲官网](https://alayacare.com/en-au/) | 成熟的端到端平台和已有澳洲 aged-care 客户/渠道，对 careKind 的平台化扩张构成竞争；但核心优势是全套软件，不是独立护士语音 scribe。逐项确认澳洲各模块实际可用性与 CMS 接入。 |
| **Kernl** | 面向 aged care 与 disability providers 的 frontline workflow / point-of-care intelligence | 统一 shift notes、reports、observations、timesheets；对话式 AI 引导员工按组织标准记录，生成 care plans，分析趋势并提示风险；网站称能减少 70% reporting 工作（供应商自述）。 [官网](https://kernl.com.au/) | 强调全班次覆盖、记录之后的趋势洞察，而非单纯生成一条 note。品牌同时覆盖 NDIS，需核实 residential aged care 的具体流程、临床治理和部署证据。 |
| **Docca** | 澳大利亚跨领域 AI clinical documentation（含 aged care、NDIS、心理健康、GP） | 生成 progress notes、plans、assessments、incident reports；可将用户上传的既有模板转换为 AI 模板。 [官网](https://docca.io/?locale=en_AU) | 模板灵活、跨专业，适合小型服务商或个人临床人员；公开页面没有清楚证明 ambient aged-care shift capture 或与主流 aged-care CMS 的原生回写。 |
| **Vira / AIDA** | 面向 aged care facilities 的 AI 文书和 AN-ACC funding 优化 | 网站称可与 Leecare、iCare 集成、实时检查临床记录并给出合规提示及 funding insights；页面宣传 23% 平均 funding 增长等指标。 [官网](https://vira.au/) | 明确把文书质量与 funding capture 结合，属于直接竞争定位。性能数字、客户引语、集成深度没有在该页面附独立证据，应视为未核实营销声明；不宜把“提高 funding”承诺作为 careKind 的核心宣传，需以记录准确和减负为主。 |
| **Heidi Health** | 澳大利亚起源的通用 AI medical scribe，官网现设 aged-care 场景 | 转录临床对话、按模板生成可编辑笔记，并基于笔记生成后续文件；aged-care 页面覆盖护士、care partners、社区支持、伤口文书等。 [Aged care 页面](https://www.heidihealth.com/solutions/aged-care)；[产品说明](https://support.heidihealth.com/en/articles/8885059-what-is-heidi) | 品牌知名度和通用 scribe 能力强，可能由个别从业人员或机构试用；仍需验证 residential 轮班记录、多人/多 resident 工作流、aged-care CMS 写回和机构级管控是否匹配。 |

## 既有系统：相邻竞争与潜在集成对象

- **Telstra Health（Clinical Manager、CareKeeper）**：成熟 residential 软件组合，覆盖临床管理、移动端床旁记录、药物、住民行政和家庭沟通。CareKeeper 支持工作人员在 resident 身边用移动设备记录。其产品以数字记录流程为主，当前公开 aged-care 页面未显示专用生成式 AI 文书功能。 [Aged care portfolio](https://www.telstrahealth.com/sectors/aged-care/)
- **Person Centred Software（mCare）**：移动临床记录系统，支持 person-centred care plans、risk assessments、charts 等，可从单一机构扩展到大型组织。公开产品页未显示 AI 文书能力。 [mCare](https://personcentredsoftware.com/en-au/products/clinical-care-system)
- **Leecare（Platinum6）**：aged/community care 临床、照护及生活管理平台；其网页强调评估、报告和 care plan 之间数据连贯、减少重复录入，并提供 point-of-care 移动应用。公开介绍未表明有 AI scribe。 [Care delivery management](https://www.leecare.com.au/index.php/care-delivery-management/)

这些 incumbents 通常比新 AI 工具更接近正式 resident record。careKind 可优先探索“经护士审核后写回既有系统”的轻量集成，而不是要求机构先替换核心 CMS。ADHA 的 residential aged-care 数字健康计划正在推动临床系统与 My Health Record / Aged Care Transfer Summary 的互通，选择结构化数据、审计和可导出的架构会减少后续接入阻力。 [ADHA：Residential aged care](https://www.digitalhealth.gov.au/healthcare-providers/residential-aged-care)；[临床系统标准说明](https://www.digitalhealth.gov.au/sites/default/files/documents/clinical-information-systems-for-residential-aged-care-fact-sheet.pdf)

## 对 careKind AI 的机会

1. **从护士最耗时的 aged-care 记录切入。** 先做好 progress note、shift handover、incident report、观察/food-fluid 记录等高频文书；让护士口述或简短输入后得到结构清晰的草稿，并明确区分“观察事实、住民/家属原话、采取的措施、待跟进事项”。
2. **嵌入班次和 resident 流程。** 竞争者已覆盖语音转写、模板、摘要、趋势分析。可用更贴近澳洲 aged-care 工作的多 resident shift 队列、遗漏项提醒、交接摘要与易用的审核回写来建立差异；提醒只能指出缺失或来源内容，不应擅自补造临床事实。
3. **让人类审核和来源追踪成为产品基础。** TGA 对 digital scribe 的说明指出，满足定义的 digital scribe 供应前须纳入 ARTG；若产品解释临床谈话并生成未由专业人员明确提出的诊断、鉴别诊断或治疗建议，则可能构成医疗器械。专业人员仍须取得知情同意并核对记录准确性。设计产品时先把功能边界、审核确认、录音同意、纠错历史、访问控制和证据来源做清楚，并让法规专家按具体功能确认分类。 [TGA：Digital scribes](https://www.tga.gov.au/products/medical-devices/software-and-artificial-intelligence-ai/overview/types-software-based-medical-devices/digital-scribes)
4. **以集成和可验证的质量指标竞争。** 与 CMS 厂商竞争替换成本高；提供草稿导出/安全回写、标准化模板映射和审计记录。试点应测量每条记录耗时、护士编辑率、遗漏/幻觉率、交接可读性和记录完成率，先发布实测结果，再使用节省时间等宣传数字。
5. **谨慎处理商业回报承诺。** 部分竞争者将文书 AI 与 AN-ACC funding 绑定。careKind 可以帮助记录准确反映护理需求，但不要暗示 AI 能决定分类或保证 funding 增长；护士与评估流程要保留专业判断。

## 公开定价与证据限制

本次查阅的相关产品页面没有发现可直接比较的公开企业订阅价格。Notive 页面提供 7 日试用，后续称按机构规模协商；Docca 标示免费开始。其他产品通常引导预约演示。所有“合规”“节省时间”“提高 funding”“高准确率”等均按厂商声明记录；签约前要求现场演示、客户推荐、数据处理与保留条款、澳洲数据流图、渗透测试/认证范围、事故响应承诺、产品责任保险、AI 输出日志和正式集成清单。

