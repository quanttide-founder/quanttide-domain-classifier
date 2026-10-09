# 分类目标数据：领域第二大脑名单

`quanttide-repo-classifier` 的分类目标类别表：待分类仓库按下表归入对应领域第二大脑。

- 数据来源：`quanttide/quanttide` 的 `domains/README.md`（领域清单与目录树）与 `.gitmodules`（`domains/` 子模块）
- 采集日期：2026-10-10
- 类别总数：45 个已建仓领域，5 个已定义未建仓领域

## 已建仓领域

| 分组 | 领域 | 英文命名 | 缩写 | 仓库 | 描述 |
| --- | --- | --- | --- | --- | --- |
| 核心技术工程 | 智能体工程 | agent-engineering | `agent` | `domains/quanttide-agent` | 侧重多智能体与人机协作。 |
| 核心技术工程 | 课程研发 | course-development | `course` | `domains/quanttide-course` | 课程研发全生命周期的工程化实践。 |
| 核心技术工程 | 数据工程 | data-engineering | `data` | `domains/quanttide-data` | 数据采集、存储、处理与服务的工程化实践。 |
| 核心技术工程 | 交互设计 | interaction-design | `ixd` | `domains/quanttide-design` | 产品界面布局与交互流程的设计工程化实践。 |
| 核心技术工程 | 文档工程 | document-engineering | `docs` | `domains/quanttide-docs` | 文档的写作、组织、发布与访问工程化实践。 |
| 核心技术工程 | 基础设施 | infrastructure | `infra` | `domains/quanttide-infra` | 侧重 IaaS 的标准化。 |
| 核心技术工程 | 知识工程 | knowledge-engineering | `knowl` | `domains/quanttide-knowl` | 知识表示、建模、推理与应用的工程化实践。 |
| 核心技术工程 | 元工程 | meta-engineering | `meta` | `domains/quanttide-meta` | 哲学的实现：把哲学命题落成可运行的结构、规则与工具。 |
| 核心技术工程 | 搜索工程 | search-engineering | `search` | `domains/quanttide-search` | 索引、召回与排序的工程化实践。 |
| 核心技术工程 | 安全工程 | security-engineering | `sec` | `domains/quanttide-security` | 网络、应用与数据安全的防护与运营工程化实践。 |
| 核心技术工程 | 知识工作 | knowledge-work | `work` | `domains/quanttide-work` | 知识工作方法、流程与工具的知识体系。 |
| 核心技术工程 | 写作管理 | narrative-engineering | `writing` | `domains/quanttide-write` | 面向内容创作者的写作流程管理。 |
| 沟通与管理 | 沟通管理 | communication-management | `comm` | `domains/quanttide-connect` | 组织内外部沟通的标准化管理。 |
| 沟通与管理 | 议事管理 | deliberation-management | `delib` | `domains/quanttide-delib` | 会议、决议与集体决策过程管理。 |
| 沟通与管理 | 语言分析 | language-analysis | `language` | `domains/quanttide-language` | 语言的结构、意义与用法的分析与应用。 |
| 职能与人力 | 财务管理 | finance-management | `finance` | `domains/quanttide-finance` | 预算、核算、税务管理。 |
| 职能与人力 | 增长管理 | growth-management | `growth` | `domains/quanttide-growth` | 增长策略、增长实验与增长效果的标准化管理。 |
| 职能与人力 | 健康管理 | health-management | `health` | `domains/quanttide-health` | 身心健康平衡管理，面向个人、家庭与企业。 |
| 职能与人力 | 人力资源 | human-resources | `hr` | `domains/quanttide-human` | 组织架构、招聘、绩效管理。 |
| 职能与人力 | 学习管理 | learning-management | `learn` | `domains/quanttide-learn` | 学习路径、进度与效果的标准化管理。 |
| 职能与人力 | 项目管理 | project-management | `project` | `domains/quanttide-project` | 项目全周期管理。 |
| 职能与人力 | 学术研究 | academic-research | `research` | `domains/quanttide-research` | 学术成果、研究项目与学术交流的标准化管理。 |
| 业务与客户 | 算法工程 | algorithm-engineering | `alg` | `domains/quanttide-algorithm` | 算法开发与部署工程化。 |
| 业务与客户 | 商务拓展 | business-development | `bd` | `domains/quanttide-business` | 合作伙伴关系与市场开拓。 |
| 业务与客户 | 信用管理 | credit-management | `credit` | `domains/quanttide-credit` | 主体与交易的信用评价、信用记录与信用治理。 |
| 业务与客户 | 众包管理 | crowd-sourcing | `crowd` | `domains/quanttide-crowd` | 众包市场的发单、接单、标准交易与信用沉淀。 |
| 业务与客户 | 客户关系 | customer-relations | `crm` | `domains/quanttide-customer` | 客户信息与销售过程管理。 |
| 业务与客户 | 创业管理 | entrepreneurship-management | `entrep` | `domains/quanttide-entrep` | 从创业想法到企业成立与早期成长的经营过程管理。 |
| 业务与客户 | 支付工程 | payment-engineering | `pay` | `domains/quanttide-pay` | 支付流程与账务处理。 |
| 业务与客户 | 密码管理 | secret-management | `secret` | `domains/quanttide-secret` | 凭证、密钥与敏感信息的全生命周期管理。 |
| 品牌与运营 | 新媒体运营 | social-media | `media` | `domains/quanttide-media` | 社交媒体矩阵运营。 |
| 品牌与运营 | 公共关系 | public-relations | `pr` | `domains/quanttide-relation` | 媒体关系与危机应对。 |
| 未分组 | 资产管理 | — | `—` | `domains/quanttide-asset` | 量潮数字资产管理 |
| 未分组 | 身份认证 | — | `—` | `domains/quanttide-auth` | 量潮身份认证 — 统一身份与权限管理 |
| 未分组 | 软件工程 | — | `—` | `domains/quanttide-code` | 量潮软件工程 |
| 未分组 | DevOps 工程 | — | `—` | `domains/quanttide-devops` | 量潮DevOps第二大脑 |
| 未分组 | 经济建模 | — | `—` | `domains/quanttide-econ` | 量潮经济建模 |
| 未分组 | 执行管理 | — | `—` | `domains/quanttide-execute` | 量潮执行工程 — 任务执行与流程编排 |
| 未分组 | 创新管理 | — | `—` | `domains/quanttide-innov` | 量潮创新管理 |
| 未分组 | 组织管理 | — | `—` | `domains/quanttide-org` | 量潮组织管理 — 组织架构与行政管理 |
| 未分组 | 产品研发 | — | `—` | `domains/quanttide-product` | 量潮产品研发领域 |
| 未分组 | 销售管理 | — | `—` | `domains/quanttide-sales` | 量潮销售管理领域知识仓库 |
| 未分组 | 战略管理 | — | `—` | `domains/quanttide-strategy` | 量潮战略管理 |
| 未分组 | 客户支持 | — | `—` | `domains/quanttide-support` | 量潮客户支持第二大脑 |
| 未分组 | 认知工程 | — | `—` | `domains/quanttide-think` | 量潮认知工程 |

## 已定义未建仓领域

领域清单中已定义、`domains/` 下尚无对应仓库的类别，作为预留目标。

| 分组 | 领域 | 英文命名 | 缩写 | 描述 |
| --- | --- | --- | --- | --- |
| 沟通与管理 | 行政管理 | administration-management | `admin` | 日常行政事务、资产管理。 |
| 职能与人力 | 法务管理 | legal-management | `legal` | 合同、合规与风险控制。 |
| 业务与客户 | 数字身份 | identity-management | `iam` | 统一身份与权限管理。 |
| 品牌与运营 | 品牌管理 | brand-management | `brand` | 品牌定位与视觉识别。 |
| 品牌与运营 | 社群运营 | social-group | `group` | 私域社群组织与运营。 |

## 分类规则

1. 以仓库名与描述为分类依据，优先匹配上表的仓库名与缩写。
2. 跨领域仓库按主体归属判定，与 `quanttide/quanttide` 的四轴划分（assets / domains / default / adapters）保持一致。
3. 无匹配类别时归入 `未分类`，并在此表新增候选类别后重跑分类。
