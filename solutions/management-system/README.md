# Governance Domain: Management System 治理域：管理体系

## Domain Scope

This domain defines the top-level control architecture of the laboratory's quality management system. It does not manage a specific asset (like data or equipment) but provides the structural logic that ensures all other governance domains operate as a cohesive system.

It answers: "How should the management system itself function as a control system?"

## Core Questions This Domain Answers
1. What are the control layers of the management system?
2. How does information flow between layers?
3. How are decisions escalated from operations to strategy?
4. How do other governance domains fit into this architecture?

## Core Outputs

|Artifact|Description|
|--------|-----------|
|control-architecture.drawio|Four-layer control architecture diagram|
|control-model.md|Detailed control logic for each layer|
|escalation-path.drawio|Information escalation workflow|

## Relationship to Other Domains

This is a meta-governance domain. It defines the operating rules for the entire system. All other domains (data/, personnel/, equipment/, etc.) operate within this architecture. Their specific control models should align with the escalation and feedback logic defined here.


## 域范围

本域定义实验室质量管理体系的顶层控制架构。它不管理某一类具体资产（如数据或设备），而是提供确保所有其他治理域作为一个连贯系统运行的结构逻辑。

它回答的是："管理体系本身应如何作为一个控制系统运作？"

## 本域回答的核心问题

1. 管理体系的控制层有哪些？
2. 信息如何在各层之间流动？
3. 决策如何从运营层升级到战略层？
4. 其他治理域如何适配到这个架构中？

## 核心产出物

|产出物|描述|
|------|----|
|control-architecture.drawio|四层控制架构图|
|control-model.md|每层的详细控制逻辑|
|escalation-path.drawio|信息升级工作流|

## 与其他域的关系

这是一个元治理域。它为整个系统定义运行规则。所有其他域（data/、personnel/、equipment/ 等）都在此架构内运行。它们各自的控制模型应与本域定义的升级和反馈逻辑对齐。
