# TRAE 项目规则:thoughtspace-arcade

> L3 项目规则 - 父级: ../CLAUDE.md(L1 宪法)
> 本文件供 TRAE 直接加载,凡 AI 助手在本项目工作时必须遵守。

## 当前所处阶段
🚧 占位阶段 - 笔记路线 wcaca/thoughtspace-notes 完成 Phase 1 后才启动本仓库。

## 共享约束
- 产品灵魂、架构原则、术语表 — 同步 wcaca/thoughtspace-notes/CLAUDE.md
- 任何违背 notes L1 的改动,在这里视为违背 arcade
- 本文件内容与 notes 项目规则同步手工复制,不需要重新起草

## 强制约束(来自 L1,完整清单)

### 架构
1. `src/core/**` 禁止 import 任何渲染库(pixi.js)
2. `src/core/**` 禁止 import `src/{render, ui, persistence, sim}` 任何模块
3. `src/sim/**` 禁止 import `src/{render, ui}` 任何模块

### 文档(GEB 协议)
4. 修改代码时:改完必更新该文件的 L3 头部
5. 修改目录时:增/删文件必更新所在目录 CLAUDE.md
6. 修改顶层结构时:必同步 L1
7. 新建目录时:必创建该目录的 CLAUDE.md

### 产品
8. 不做数值化等级/积分
9. AI 自动化建议必须以"半透明预览"形式呈现
10. 笔记内容默认不上云

## 工作流
11. 每次代码变更前必跑:`npm run check:arch && npm test`
12. 每次 commit 前 L3 → L2 → L1 三层回环检查
13. commit message 必须含 `spec-id: ...` 与 `task-id: ...` 字段

## 输出风格
- 思考: 英文
- 交互: 中文
- 注释: 中文 + ASCII 分块

[PROTOCOL]: 变更时更新此头部,然后检查 ../../CLAUDE.md
