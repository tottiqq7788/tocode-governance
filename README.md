# tocode · 治理控制面（governance）

本目录是 `tocode` 项目的治理控制面（文件型），由 Agent 持续分析、管理、更新，并按其中流程与用户沟通。

## 目录定位

- 规范内核：`/Users/admin/totti/project/public/agent-governance`（Agent Governance Kit v0.1.0）。
- 本目录是项目根目录下**唯一强制**的子文件夹；其余子文件夹（product / frontend / backend 等）按最终需求与技术栈，在开发执行前再初始化。

## 文件夹约定（用户硬性偏好）

- 项目根目录不放杂乱文件、不建 `.git`，只放若干子文件夹。
- 子文件夹按角色 / 技术栈划分；`governance/` 是控制面。
- 每个子文件夹独立 git 管理。

## 当前状态

- project_id：`tocode`
- mode：`new`（全新项目，先定义语义再开发）
- baseline：冻结于脚手架提交（见 `architecture/governance.json`）

## 权威入口

- 治理清单：`architecture/governance.json`
- 语义地图：`architecture/traceability/semantic-map.json`
- 架构合同：`architecture/contracts/`
- Inventory：`architecture/inventories/`
- 工作包：`architecture/work-packages/`
- 证据：`architecture/evidence/`

## 校验

```text
python3 architecture/tools/audit_project.py --target .
```
