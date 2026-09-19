# AUR Packages Helper（已归档）

> ⚠️ 本项目已合并进 [aur-packages](https://github.com/awsl1414/aur-packages)（`projects/aur-metadata`），本仓库不再维护，仅作历史存档。

## 说明

`aur-packages-helper` 曾是 [aur-packages](https://github.com/awsl1414/aur-packages) 的配套服务，负责获取应用版本、计算文件 hash 等辅助功能。现已作为 `aur-metadata` 成员并入 aur-packages monorepo，后续所有开发、Issue 与 PR 请前往：

- **新仓库**：https://github.com/awsl1414/aur-packages
- **新位置**：[`projects/aur-metadata`](https://github.com/awsl1414/aur-packages/tree/dev/projects/aur-metadata)

## 原功能概述

- FastAPI 查询服务：追踪上游应用版本、计算文件 hash
- Tortoise ORM + SQLite 持久化，APScheduler 定时采集
- 版本与 hash 独立采集、独立落库，快照过期时后台异步刷新，查询纯读数据库不阻塞

## 技术栈（历史）

Python 3.13+ / uv · FastAPI · Tortoise ORM · APScheduler
