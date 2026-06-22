# Control Model: Four-Layer Control Architecture 控制模型：四层控制架构

## Core Principle

A management system is a control system. Its purpose is to ensure that operations stay within defined boundaries and that the system adapts when boundaries are challenged. This model defines four layers of control, each with a distinct function, connected by information flows.

## The Four Layers

```text
┌─────────────────────────────────────────────────────────────┐
│ Layer 1: STRATEGIC CONTROL                                │
│ Function: Set direction, allocate resources, adjust system │
│ Activities: Management review, policy setting, resource   │
│ allocation, responding to external changes                │
│ Inputs: System performance summaries, trends, external    │
│ changes, client feedback                                  │
│ Outputs: Strategic decisions, resource reallocation,      │
│ policy updates                                            │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ Information flow
                              │ │ (up: escalation, down: policy)
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ Layer 2: CORRECTIVE CONTROL                               │
│ Function: Detect deviations, analyze root causes, apply   │
│ corrections and preventive actions                       │
│ Activities: CAPA, nonconformance management, complaint    │
│ handling, root cause analysis                             │
│ Inputs: Nonconformance reports, audit findings,          │
│ complaint data, performance deviations                   │
│ Outputs: Corrective actions, preventive actions,         │
│ procedure updates, training changes                      │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ Information flow
                              │ │ (up: findings, down: instructions)
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ Layer 3: DIAGNOSTIC CONTROL                               │
│ Function: Periodically check system health, identify      │
│ issues before they become failures                        │
│ Activities: Internal audit, routine supervision,          │
│ equipment verification, document review                   │
│ Inputs: Audit plans, checklists, operational records,     │
│ system logs                                               │
│ Outputs: Audit findings, improvement areas, early         │
│ warnings, conformity confirmations                        │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ Information flow
                              │ │ (up: deviations, down: standards)
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ Layer 4: EXECUTION CONTROL                                │
│ Function: Ensure daily operations are performed within    │
│ defined controls                                          │
│ Activities: Training, equipment use & calibration,        │
│ document control, sample management, method execution,    │
│ data recording                                            │
│ Inputs: SOPs, work instructions, training records,        │
│ equipment logs                                            │
│ Outputs: Operational records, raw data, nonconformance    │
│ reports, training feedback                                │
└─────────────────────────────────────────────────────────────┘
```

## Layer Details

### Layer 1: Strategic Control

**Role**: This is the decision-making layer. It evaluates the overall performance of the system, identifies gaps between current capability and future requirements, and makes decisions to adjust direction or allocate resources.

The Question It Answers: "Are we doing the right things?"

**Key Activities**:

- Conducting management review meetings
- Setting quality objectives and policies
- Responding to changes in regulations, client needs, or market conditions
- Allocating budget, personnel, and infrastructure

Information It Needs: System-level summaries (not raw data), trend analysis, risk assessments, client feedback, external changes.

Information It Produces: Strategic decisions, resource allocations, policy changes, updated objectives.

### Layer 2: Corrective Control

**Role**: This layer is activated by deviations or failures. Its goal is not just to fix the immediate issue but to identify the systemic cause and prevent recurrence.

The Question It Answers: "Why did this happen, and how do we stop it from happening again?"

**Key Activities**:

- Investigating nonconformances
- Conducting root cause analysis
- Implementing corrective and preventive actions (CAPA)
- Verifying the effectiveness of actions taken

Information It Needs: Nonconformance reports, audit findings, client complaints, operational deviations.

Information It Produces: Corrective actions, preventive actions, updates to procedures or training, input for management review.

### Layer 3: Diagnostic Control

**Role**: This layer provides a periodic "health check" of the system. It operates independently of daily operations to provide an objective view of whether the system is functioning as designed.

The Question It Answers: "Is our system working as intended?"

**Key Activities*:

- Planning and conducting internal audits
- Performing routine supervision
- Conducting equipment performance verification (intermediate checks)
- Reviewing documents for effectiveness

Information It Needs: Audit plans, work instructions, operational records, system logs.

Information It Produces: Audit findings, improvement areas, early warnings, confirmation of conformity.

### Layer 4: Execution Control

**Role**: This layer is embedded in routine work. Its goal is to prevent deviations by ensuring every task is performed correctly by trained personnel using validated methods and calibrated equipment.

The Question It Answers: "Are we doing things right?"

**Key Activities**:
- Managing training and competence
- Operating equipment with proper calibration and maintenance
- Following document control procedures
- Executing sample management and methods
- Recording data correctly and completely

Information It Needs: SOPs, work instructions, training records, equipment logs.

Information It Produces: Operational records, raw data, nonconformance reports, training feedback.

## Information Flow and Escalation
The effectiveness of this architecture depends on information flowing between layers. The key principle is escalation:

|Flow Direction|Path|Purpose|
|--------------|----|-------|
|Upward|Execution → Diagnostic|When routine checks identify execution issues, or when operational records show consistent deviations, diagnostic control investigates.|
|Upward|Diagnostic → Corrective|Audit findings or supervision observations trigger CAPA if issues are significant or recurring.|
|Upward|Corrective → Strategic|Analysis of recurring nonconformances, high-risk issues, or resource gaps is escalated to management review for strategic decisions.|
|Downward|Strategic → All Layers|Strategic decisions and resource allocations are translated into policy changes, procedure updates, and revised objectives that cascade through all layers.|

This upward flow ensures that problems at the operational level can drive changes at the policy and resource level. The downward flow of decisions ensures that strategy drives execution.

核心原则
管理体系是一个控制系统。其目的是确保运营保持在既定边界内，并且当边界受到挑战时系统能够适应。本模型定义了四个控制层，每层具有不同的功能，通过信息流相互连接。

四层架构
```text
┌─────────────────────────────────────────────────────────────┐
│ 第一层：战略层控制                                         │
│ 功能：设定方向、分配资源、调整体系                         │
│ 活动：管理评审、政策制定、资源配置、应对外部变化           │
│ 输入：系统表现摘要、趋势、外部变化、客户反馈               │
│ 输出：战略决策、资源重新配置、政策更新                     │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ 信息流
                              │ │ （上行：升级，下行：政策）
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ 第二层：校正层控制                                         │
│ 功能：检测偏差、分析根因、实施纠正与预防措施               │
│ 活动：CAPA、不符合管理、投诉处理、根本原因分析             │
│ 输入：不符合报告、审核发现、投诉数据、绩效偏差             │
│ 输出：纠正措施、预防措施、程序更新、培训变更               │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ 信息流
                              │ │ （上行：发现，下行：指令）
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ 第三层：诊断层控制                                         │
│ 功能：定期检查系统健康，在问题演变为失效前识别问题         │
│ 活动：内部审核、日常监督、设备核查、文件评审               │
│ 输入：审核计划、检查表、运行记录、系统日志                 │
│ 输出：审核发现、改进领域、早期预警、符合性确认             │
└─────────────────────────────────────────────────────────────┘
                              ▲ │
                              │ │ 信息流
                              │ │ （上行：偏差，下行：标准）
                              │ ▼
┌─────────────────────────────────────────────────────────────┐
│ 第四层：执行层控制                                         │
│ 功能：确保日常操作在既定控制措施内执行                     │
│ 活动：培训、设备使用与校准、文件控制、样品管理、           │
│       方法执行、数据记录                                   │
│ 输入：SOP、作业指导书、培训记录、设备日志                  │
│ 输出：运行记录、原始数据、不符合报告、培训反馈             │
└─────────────────────────────────────────────────────────────┘
```

## 各层详解

### 第一层：战略层控制

**角色**：这是决策层。它评估系统的整体表现，识别当前能力与未来需求之间的差距，并做出调整方向或分配资源的决策。

回答的问题："我们是否在做正确的事？"

**关键活动**：
- 召开管理评审会议
- 制定质量目标和方针
- 应对法规、客户需求或市场状况的变化
- 分配预算、人员和基础设施

需要的信息：系统级摘要（非原始数据）、趋势分析、风险评估、客户反馈、外部变化。

产出的信息：战略决策、资源分配、政策变更、更新后的目标。

### 第二层：校正层控制

**角色**：本层由偏差或失效触发。其目标不仅是修复眼前的问题，而是识别系统性原因并防止复发。

回答的问题："为什么会发生，如何阻止它再次发生？"

**关键活动**：

- 调查不符合项
- 进行根本原因分析
- 实施纠正与预防措施（CAPA）
- 验证所采取措施的有效性

需要的信息：不符合报告、审核发现、客户投诉、运营偏差。

产出的信息：纠正措施、预防措施、程序或培训的更新、为管理评审提供的输入。

### 第三层：诊断层控制

**角色**：本层提供体系的定期"健康检查"。它独立于日常运营运行，以提供关于体系是否按设计运行的客观视图。

回答的问题："我们的系统是否按预期工作？"

**关键活动**：
- 策划和实施内部审核
- 进行日常监督
- 进行设备性能核查（期间核查）
- 评审文件的有效性

需要的信息：审核计划、作业指导书、运行记录、系统日志。

产出的信息：审核发现、改进领域、早期预警、符合性确认。

### 第四层：执行层控制

**角色**：本层嵌入在例行工作中。其目标是通过确保每项任务都由经过培训的人员、使用经过验证的方法和校准过的设备正确执行，来防止偏差。

回答的问题："我们是否正确地做事？"

**关键活动**：
- 管理培训和能力
- 操作设备并进行适当的校准和维护
- 遵循文件控制程序
- 执行样品管理和检测方法
- 正确完整地记录数据

需要的信息：SOP、作业指导书、培训记录、设备日志。

产出的信息：运行记录、原始数据、不符合报告、培训反馈。

## 信息流动与升级

本架构的有效性取决于各层之间的信息流动。关键原则是升级：

|流向|路径|目的|
|----|----|----|
|上行|执行层 → 诊断层|当日常检查发现执行层问题，或运行记录显示持续偏差时，诊断层进行调查。|
|上行|诊断层 → 校正层|如果问题重要或重复发生，审核发现或监督观察结果触发CAPA。|
|上行|校正层 → 战略层|对重复发生的不符合、高风险问题或资源缺口的分析，升级到管理评审以进行战略决策。|
|下行|战略层 → 所有层|战略决策和资源分配被转化为政策变更、程序更新和修订后的目标，贯穿所有层级。|

这种上行流动确保操作层面的问题能够驱动政策和资源层面的变革。决策的下行流动确保战略驱动执行。