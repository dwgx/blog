---
title: SkiAPI 开发之旅 — 统一 AI 网关的故事
date: 2026-04-14
tags: [skiapi, AI, python, gateway]
author: DWGX
---

# SkiAPI — Born for the creation

SkiAPI (YuKiKo) 是一个统一的 AI 模型网关，一个接口接入所有主流大模型。

## Why

在使用各种 AI 模型的过程中，每个平台都有不同的 API 格式，切换模型需要改代码。SkiAPI 解决了这个问题：

- **OpenAI Compatible** — 统一的接口格式
- **Multi-model** — GPT-4o, Claude, Gemini, DeepSeek, Qwen...
- **Token Management** — 用量统计和按量计费

## Architecture

基于 NewAPI 框架，使用 Python 构建，支持：

1. 请求路由和负载均衡
2. 多 Key 轮询
3. 实时用量监控
4. 自定义模型映射

## Stats

- ★ 21 stars on GitHub
- 50+ 支持的模型
- 活跃的用户社区

Check it out: [skiapi.dev](https://skiapi.dev)
