---
title: 近期更新 · 6 月 Devlog
date: 2026-06-29
tags: [devlog, updates, vr, reverse-engineering]
author: DWGX
size: full
type: log
pin: true
color: "#6e56cf"
---

## 这阵子在忙什么

把最近两周各个仓库的更新记录梳理了一下,基本围着 **VR 逆向**、**AI 工具链** 和 **桌面工具** 三条线在推进。

### 🥽 VR / 逆向

- **VirtualDesktop** — VR 串流 App 的离线 LAN 补丁工程收尾。在 .NET IL 字节层做了 44 处精确手术,删掉 AOT 触发 JIT 回退,把"验证失败就自杀"的指令逐一 NOP 掉,顺手把界面汉化成简体中文,出可直接安装的中文 APK。配了一个介绍站讲完整工程史。
- **vrchat-il2cpp-re** ★9 — VRChat IL2CPP 反混淆管线,Unity 6 (6000.0.60f1) 基线。逆向 MethodInfo 枚举,跑到 64K 类 / 570K 方法 / 188K 字段的可复现命名。
- **VRCSM** ★3 — VRChat 设定管理器,缓存清理、设定备份迁移与诊断,Windows 端。
- **UltimateTracker_FirmWare** — VIVE Ultimate Tracker 固件与更新器研究归档(私有)。
- **Quest-ADB-Dashboard** — Meta Quest ADB 诊断面板,导出脱敏可分享的 HTML 报告。
- **VRC-Auto-Uploader** — VRChat 模型批量上传,对接 Unity + VRCSDK 创作流。

### 🤖 AI 工具链

- **WindsurfAPI** ★2859 — Windsurf 的 LLM API 代理,同时兼容 OpenAI 与 Anthropic 接口。
- **YuKiKo** ★21 — AI QQ 机器人,OneBot / NapCat + LLM 路由、插件与 WebUI。
- **CEGM** ★2 — LLM 驱动的 Cheat Engine 层,带 MCP HTTP 与本地仪表板,单机离线实验用。
- **debugger-workstation** — 便携式逆向 / 安全分析 / 调试 / MCP 自动化工作站。
- **AgentScope** — 监控本地 Codex 与 Claude Code 会话的 Windows 桌面控制台。
- **claude-codex-subagent** ★2 — Claude Code 技能,把限定范围的子任务委派给本地 Codex CLI。
- **blender-copilot** — Blender MCP 服务器,70+ 工具,面向 AI 3D 创作与 VRChat 模型工作流。
- **SKIBOX** ★2 — AI 开发工具的本地 API key 管理与配置切换器。

### 🛠️ 桌面 / 其他

- **luncher** — Windows 桌面游戏启动器(Skia + Clay + Rust 后端)。
- **JeeBacode** — 基于 Opencode 的终端 AI 编码 agent,带路由、技能、插件与子 agent。
- **DWGX** ★2 — 个人主页 / dwgx.menu,本站点。

## 接下来

VirtualDesktop 跟版本走到 1.34,会继续跟新版;vrchat-il2cpp-re 的命名管线还在补 Unity 6 的偏移。其余工具按需迭代。

> 完整提交记录都在 [github.com/dwgx](https://github.com/dwgx)。
