---
name: commit-message
description: 根据改动生成规范化的 Git 提交信息（Conventional Commits 风格）。当用户要写 commit/提交信息时使用。
when_to_use: 用户说"帮我写 commit""生成提交信息""这次改了啥写个提交"时。
---

# Git 提交信息生成

根据当前改动生成规范、清晰的提交信息。

## 步骤

1. 用 bash 跑 `git diff --staged`（无暂存则 `git diff`）看改动。
2. 跑 `git status` 看新增/删除文件。
3. 归纳改动**意图**（不是罗列文件），生成提交信息。

## 格式（Conventional Commits）

```
<type>(<scope>): <简短描述>

<可选正文：为什么改，而非改了什么>
```

## type 取值

- feat: 新功能
- fix: 修 bug
- docs: 文档
- style: 格式（不影响逻辑）
- refactor: 重构
- perf: 性能
- test: 测试
- chore: 构建/工具
- ci / build / revert

## 规则

- 标题 ≤ 50 字，**中文**，动宾结构，结尾不加句号。
- 一个 commit 只做一件事；若改动混杂，提示用户拆分。
- 正文解释"为什么"，不重复标题。

## 输出

先给推荐信息（可直接复制），再附一句"如需调整 type/scope 告诉我"。