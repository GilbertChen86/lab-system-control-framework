# **Architecture Overview: Four-Layer Control Architecture**

## 1. Design Philosophy

This architecture is built on the fundamental understanding that a management system is a control system. Its purpose is not to accumulate documents, but to ensure that the organization's operations remain within defined boundaries and can adapt to changes. The design follows three core principles:

- Control Loops: Every management activity should be designed as a closed-loop control system with five essential elements: Sense → Judge → Decide → Execute → Feedback.

- Layered Structure: Control functions are distributed across four distinct but interconnected layers, each with a specific role in the overall system.

- Information Flow: The primary purpose of the architecture is to ensure that information about system performance flows upward for decision-making, and strategic decisions flow downward to drive execution and adjustment.

## 2. The Four Layers

The architecture consists of four control layers, ordered from strategic to operational:

### Layer 1: Strategic Control

**Primary Function**: To set the overall direction, allocate resources, and make decisions about the evolution of the management system itself.

**Key Activities**:

- Management Review
- Defining quality objectives and policies
- Responding to changes in the external environment (regulations, client needs, market conditions) 
- Resource allocation (budget, personnel, infrastructure)

**Control Logic**: This layer evaluates the system's overall performance, identifies gaps between current capability and future requirements, and makes decisions to adjust the system's direction or resource base. It is the layer where the question "Are we doing the right things?" is answered.

**Information Inputs**: System performance summaries, trends from other layers, external changes, client feedback.

**Information Outputs**: Strategic decisions, resource reallocation, policy changes, updated objectives.

### Layer 2: Corrective Control

**Primary Function**: To detect deviations that have already occurred, analyze their root causes, and implement actions to correct them and prevent recurrence.

**Key Activities**:

CAPA (Corrective and Preventive Actions)

- Nonconformance Management
- Customer Complaint Handling (when escalated)
- Root Cause Analysis

**Control Logic**: This layer is triggered by deviations or failures. Its goal is not just to fix the immediate issue but to identify the systemic cause and update the system to prevent similar issues in the future. It is the layer where the question "Why did this happen, and how do we stop it from happening again?" is answered.

**Information Inputs**: Nonconformance reports, audit findings, customer complaints, performance data deviations.

**Information Outputs**: Corrective actions, preventive actions, updates to procedures or training, knowledge for management review.

### Layer 3: Diagnostic Control

**Primary Function**: To periodically and systematically check the health of the management system to identify potential issues before they become failures.

**Key Activities**:

- Internal Audits
- Routine Supervision
- Equipment Performance Verification (e.g., intermediate checks)
- Document Review and Effectiveness Checks

**Control Logic**: This layer provides a "health check" of the system. It operates independently of daily operations to provide an objective view of whether the system is functioning as designed. It is the layer where the question "Is our system working as intended?" is answered.

**Information Inputs**: Audit plans, checklists, operational records, system logs.

**Information Outputs**: Audit findings, areas for improvement, confirmations of conformity, early warning signals.

### Layer 4: Execution Control

**Primary Function**: To ensure that daily operational activities are performed within the defined controls and standards.

**Key Activities**:

- Training and Competence Management
- Equipment Use, Calibration, and Maintenance
- Document Control
- Sample Management and Method Execution
- Data Recording and Archiving

**Control Logic**: This layer is embedded in the routine work of the laboratory. Its goal is to prevent deviations by ensuring that every task is performed correctly, by trained personnel, using validated methods and calibrated equipment, with proper documentation. It is the layer where the question "Are we doing things right?" is answered.

**Information Inputs**: Standard operating procedures, work instructions, training records, equipment logs.

**Information Outputs**: Operational records, raw data, nonconformance reports, training feedback.

## 3. The Connecting Logic: How Information Flows

The architecture's effectiveness depends on the flow of information between layers. The key principle is escalation:

- From Execution to Diagnostic: When routine checks (diagnostic) identify issues in execution, or when execution records show consistent deviations, this information must be escalated for systematic review.
- From Diagnostic to Corrective: Audit findings or supervision observations are inputs to the CAPA process. They trigger corrective actions if the issue is significant or recurring.
- From Corrective to Strategic: Analysis of recurring nonconformances, high-risk issues, or significant resource gaps identified through CAPA must be escalated to management review for strategic decision-making.

This upward flow ensures that problems at the operational level can drive changes at the policy and resource level. The downward flow of decisions and resource allocations from the strategic layer drives the adjustments needed at all lower layers.

## 4. Architectural Principle Summary

- Separation of Concerns: Each layer has a clear, non-overlapping function.
- Closed-Loop Design: Each key activity within a layer is a control loop with feedback.
- Upward Information Escalation: Problems detected at any level must have a path to be escalated for appropriate decision-making.
- Downward Policy Implementation: Decisions and strategic adjustments must be translated into actionable changes at the execution level.

---

# **架构概览：四层控制架构**
## 1. 设计理念

本架构基于一个基本理解：管理体系本质上是一个控制系统。其目的不是积累文件，而是确保组织的运行保持在既定边界内，并能够适应变化。设计遵循三个核心原则：

- 控制回路：每一项管理活动都应设计为一个闭环控制系统，包含五个基本要素：感知 → 判定 → 决策 → 执行 → 反馈。
- 分层结构：控制功能分布在四个不同但相互连接的层级，每个层级在整体系统中承担特定角色。
- 信息流动：该架构的主要目的是确保关于系统表现的信息上行以支持决策，而战略决策下行以驱动执行和调整。

## 2. 四个层级

该架构包含四个控制层级，按战略层到操作层的顺序排列：

### 第一层：战略层控制

**主要功能**：设定整体方向、分配资源、并对管理体系自身的演进做出决策。

**关键活动**：

- 管理评审
- 制定质量目标和方针
- 应对外部环境变化（法规、客户需求、市场状况）
- 资源分配（预算、人员、基础设施）

**控制逻辑**：该层级评估系统的整体表现，识别当前能力与未来需求之间的差距，并做出调整系统方向或资源基础的决策。这是回答“我们是否在做正确的事？”这一问题的层级。

**信息输入**：系统表现摘要、来自其他层级的趋势、外部变化、客户反馈。

**信息输出**：战略决策、资源重新配置、政策变更、更新后的目标。

### 第二层：校正层控制

**主要功能**：检测已发生的偏差，分析其根本原因，并实施纠正和预防措施。

**关键活动**：

- CAPA（纠正与预防措施）
- 不符合管理
- 客户投诉处理（当升级时）
- 根本原因分析

**控制逻辑**：该层级由偏差或失效触发。其目标不仅是修复眼前的问题，而是识别系统性原因并更新系统以防止类似问题再次发生。这是回答“为什么会发生，以及如何阻止它再次发生？”这一问题的层级。

**信息输入**：不符合报告、审核发现、客户投诉、表现数据偏差。

**信息输出**：纠正措施、预防措施、程序或培训的更新、为管理评审提供的知识。

### 第三层：诊断层控制

**主要功能**：定期、系统地检查管理体系的健康状况，以识别潜在问题，防止其演变为失效。

**关键活动**：

- 内部审核
- 日常监督
- 设备性能验证（如期间核查）
- 文件评审与有效性检查

**控制逻辑**：该层级提供体系的“健康检查”。它独立于日常运营运行，以提供关于体系是否按设计运行的客观视图。这是回答“我们的系统是否按预期工作？”这一问题的层级。

**信息输入**：审核计划、检查表、运行记录、系统日志。

**信息输出**：审核发现、改进领域、符合性确认、早期预警信号。

### 第四层：执行层控制

**主要功能**：确保日常操作活动在既定的控制措施和标准内执行。

**关键活动**：

- 培训与能力管理
- 设备使用、校准和维护
- 文件控制
- 样品管理和方法执行
- 数据记录和存档

**控制逻辑**：该层级嵌入在实验室的日常工作中。其目标是通过确保每项任务都由经过培训的人员、使用经过验证的方法和校准过的设备、并附有适当文档来正确执行，从而防止偏差。这是回答“我们是否正确地做事？”这一问题的层级。

**信息输入**：标准操作规程、作业指导书、培训记录、设备日志。

**信息输出**：运行记录、原始数据、不符合报告、培训反馈。

## 3. 连接逻辑：信息如何流动

该架构的有效性取决于各层级之间的信息流动。关键原则是升级：

- 从执行层到诊断层：当日常检查（诊断层）发现执行层的问题，或执行记录显示持续偏差时，此信息必须升级以便进行系统性审查。
- 从诊断层到校正层：审核发现或监督观察结果是CAPA流程的输入。如果问题重要或重复发生，则触发纠正措施。
- 从校正层到战略层：对重复发生的不符合、高风险问题或通过CAPA识别出的重大资源缺口的分析，必须升级到管理评审以进行战略决策。

这种上行流动确保了操作层面的问题能够驱动政策和资源层面的变革。来自战略层的决策和资源分配的下行流动，则驱动所有较低层级所需的调整。

## 4. 架构原则总结

- 关注点分离：每个层级都有清晰、不重叠的功能。
- 闭环设计：层级内的每项关键活动都是一个带有反馈的控制回路。
- 信息向上升级：在任何层级发现的问题都必须有路径升级到适当的决策层。
- 策略向下实施：决策和战略调整必须转化为执行层可操作的改变。
