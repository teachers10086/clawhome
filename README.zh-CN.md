# 龙虾之家

![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-early-blue)
![Language](https://img.shields.io/badge/lang-English%20%7C%20中文-orange)

[English](./README.md) | 中文

一个汇总 Claw 生态项目的导航仓库，用来介绍 GitHub 上具有代表性的 Claw 系开源 AI 助手项目，并说明它们的用途、适用环境、部署方式、命名差异与大致成熟度。

> ClawHome 重点收录生态中具有代表性、方向差异明显、便于理解整体格局的项目，而不是追求“绝对收全”。

---

## 目录

- [什么是 ClawHome？](#什么是-clawhome)
- [快速上手](#快速上手)
- [当前收录项目](#当前收录项目)
- [生态结构图](#生态结构图)
- [项目对比表](#项目对比表)
- [详细项目说明](#详细项目说明)
- [命名歧义说明](#命名歧义说明)
- [建议统一使用的评估维度](#建议统一使用的评估维度)
- [这个仓库适合谁？](#这个仓库适合谁)
- [贡献指南](#贡献指南)
- [Roadmap](#roadmap)
- [免责声明](#免责声明)
- [License](#license)

---

## 什么是 ClawHome？

ClawHome 是一个面向 **Claw 生态** 的导航仓库。  
这里所说的 Claw 生态，主要指围绕 **OpenClaw** 及其相关衍生项目逐步形成的一组开源 AI 助手项目，包括：

- 核心运行时
- local-first 变体
- 轻量化实现
- 嵌入式版本
- 多 Agent 编排层
- 后续可能出现的生态基础设施

这个仓库希望帮助读者快速回答这些问题：

- GitHub 上主要有哪些 Claw 项目？
- 每个项目是做什么的？
- 哪个项目更适合我的环境？
- OpenClaw、PicoClaw、MimiClaw、LocalClaw、Mimiclaw 之间有什么区别？
- 哪些适合自托管？哪些适合本地推理？哪些更偏硬件？哪些适合多 Agent？

---

## 快速上手

如果你刚接触 Claw 生态，可以这样理解：

- 选择 **[OpenClaw](https://github.com/openclaw/openclaw)**：如果你想要一个主流的、自托管的个人 AI 助手平台
- 选择 **[LocalClaw](https://github.com/sulis-dev/localclaw)**：如果你更重视本地优先和本地模型推理
- 选择 **[PicoClaw](https://github.com/sipeed/picoclaw)**：如果你想尝试轻量、低资源占用的助手运行时
- 选择 **[MimiClaw](https://github.com/memovai/mimiclaw)**：如果你想做低成本、低功耗的嵌入式 AI 助手
- 关注 **[Mimiclaw](https://github.com/Mimiclaw)**：如果你对 manager-worker 或数字员工式多 Agent 编排感兴趣

---

## 当前收录项目

当前版本重点收录以下代表性项目：

- [OpenClaw](https://github.com/openclaw/openclaw)
- [MimiClaw（`memovai/mimiclaw`）](https://github.com/memovai/mimiclaw)
- [PicoClaw](https://github.com/sipeed/picoclaw)
- [LocalClaw](https://github.com/sulis-dev/localclaw)
- [Mimiclaw](https://github.com/Mimiclaw)

随着生态变化，后续也可以继续补充更多项目、分支、注册表和相关工具。

---

## 生态结构图

### A. 核心助手运行时
这类项目的主要目标，是提供 AI 助手本体或运行时能力。

- **[OpenClaw](https://github.com/openclaw/openclaw)** — 核心自托管助手平台
- **[LocalClaw](https://github.com/sulis-dev/localclaw)** — 偏本地优先的 OpenClaw 风格变体
- **[PicoClaw](https://github.com/sipeed/picoclaw)** — 强调轻量、小体积部署的实现方向
- **[MimiClaw](https://github.com/memovai/mimiclaw)** — 面向受限硬件环境的嵌入式实现

### B. 编排 / 组织层
这类项目更关注 agent 团队、任务分工、manager-worker 结构或数字员工编排。

- **[Mimiclaw](https://github.com/Mimiclaw)** — 偏多 Agent / workforce 的方向

### C. 生态基础设施
未来可以继续收录：

- 技能注册表
- 部署工具
- 插件生态
- 文档站点
- 社区分支
- 对比和检索工具

---

## 项目对比表

| 项目 | 主要定位 | 最适合的场景 | 部署方式 | 核心特点 | 成熟度 |
|---|---|---|---|---|---|
| [OpenClaw](https://github.com/openclaw/openclaw) | 核心自托管个人助手 | 通用型个人 AI 助手 | 桌面 / 服务器 / 自托管 | 多渠道、可扩展、中心运行时 | 活跃 |
| [LocalClaw](https://github.com/sulis-dev/localclaw) | 本地优先助手变体 | 重视隐私和本地推理的用户 | 本地机器 | 降低云依赖，强调本地模型 | 早期但活跃 |
| [PicoClaw](https://github.com/sipeed/picoclaw) | 轻量助手运行时 | 边缘部署、低资源实验 | 轻量硬件 / 边缘环境 | 小体积、快速、简洁 | 早期 |
| [MimiClaw](https://github.com/memovai/mimiclaw) | 嵌入式助手 | 低成本、低功耗常开硬件助手 | 嵌入式设备 | 面向受限硬件的硬件化方向 | 早期 |
| [Mimiclaw](https://github.com/Mimiclaw) | 多 Agent 编排方向 | manager-worker / 数字员工实验 | 多 Agent 环境 | 并行执行、组织化抽象 | 实验性 |

> 说明：
> - 这里的“成熟度”是为了帮助读者理解项目所处阶段，并不是上游官方标签。
> - 这个表主要用于导航和选型参考，不代表严格测评。

---

## 详细项目说明

### 1）[OpenClaw](https://github.com/openclaw/openclaw)
**类型：** 核心运行时 / 自托管个人 AI 助手

**适合：**
- 想拥有通用型自托管助手的用户
- 想围绕一个中心运行时做扩展的开发者
- 想要多渠道接入和较完整能力的使用者

**典型环境：**
- 桌面开发机
- 家庭服务器
- 自托管服务器 / VPS

**为什么重要：**
OpenClaw 是 Claw 生态中的主要参考项目之一。很多相关项目，本质上都可以看作对 OpenClaw 路线的简化、特化或扩展。

---

### 2）[LocalClaw](https://github.com/sulis-dev/localclaw)
**类型：** local-first 的 OpenClaw 风格变体

**适合：**
- 非常重视隐私的用户
- 希望尽量依赖本地模型服务的用户
- 已经在使用本地推理栈的人

**典型环境：**
- 本地开发机
- 更离线化的工作流
- 本地 LLM 环境

**为什么重要：**
LocalClaw 代表了生态中的本地优先方向，适合希望更强掌控数据、上下文和推理链路的用户。

---

### 3）[PicoClaw](https://github.com/sipeed/picoclaw)
**类型：** 轻量级 Claw 风格助手

**适合：**
- 资源受限场景
- 边缘部署实验
- 想尝试极简助手运行时的人

**典型环境：**
- 小型硬件
- 边缘设备
- 实验型部署环境

**为什么重要：**
PicoClaw 代表了“小、快、便于部署”的方向，是 Claw 生态轻量化路线的重要样本。

---

### 4）[MimiClaw](https://github.com/memovai/mimiclaw)
**仓库命名说明：** `memovai/mimiclaw`

**类型：** 嵌入式助手实现

**适合：**
- 嵌入式 / IoT 实验
- 低成本常开助手
- 极受限硬件场景

**典型环境：**
- 嵌入式开发板
- 低功耗设备
- 硬件助手实验

**为什么重要：**
MimiClaw 代表了 Claw 生态中的硬件导向路线，也就是把 AI 助手能力进一步推向低成本、低功耗设备。

---

### 5）[Mimiclaw](https://github.com/Mimiclaw)
**类型：** 编排层 / workforce 风格多 Agent 方向

**适合：**
- 探索 manager-worker agent 架构的用户
- 想做多 Agent 协作实验的人
- 希望在助手之上构建“组织式执行系统”的开发者

**典型环境：**
- 多 Agent 实验环境
- 编排和任务分工系统
- 委派式工作流

**为什么重要：**
Mimiclaw 代表的是 AI 组织或数字劳动力方向，而不是单一助手本体。

---

## 命名歧义说明

Claw 生态里最容易让人混淆的名字之一，就是 **Mimiclaw**。

它至少可能指向两种不同含义：

### [`memovai/mimiclaw`](https://github.com/memovai/mimiclaw)
这个仓库常常被作为 **MimiClaw** 来介绍，通常对应嵌入式 / ESP32 风格方向。

### [Mimiclaw](https://github.com/Mimiclaw)
它也可能指向一个更偏多 Agent、workforce、组织化执行的方向。

为了避免误解，**ClawHome 会把这两者分开处理**。

---

## 建议统一使用的评估维度

为了方便横向对比，建议每个项目统一从以下维度描述：

- **定位**：个人助手、本地优先运行时、嵌入式助手、编排层、生态基础设施
- **技术栈**：TypeScript、Go、C、本地模型栈等
- **部署门槛**：桌面、服务器、Docker、嵌入式开发板、本地 LLM 运行时
- **交互方式**：Telegram、Slack、WhatsApp、CLI、Web、Matrix 等
- **适合场景**：个人自动化、隐私优先、本地推理、边缘部署、硬件助手、多 Agent 协作
- **成熟度**：稳定、活跃、早期、实验性

---

## 这个仓库适合谁？

ClawHome 主要适合：

- 想快速看懂 Claw 生态的开发者
- 想做项目选型的用户
- 想跟踪生态分化方向的贡献者
- 想比较自托管、本地优先、嵌入式、多 Agent 路线差异的人

---

## 贡献指南

欢迎提交 PR 一起完善这个仓库。

你可以从这些方向贡献：

- 补充遗漏的 Claw 项目
- 修正过时描述
- 优化分类体系和对比维度
- 增加部署说明
- 进一步澄清命名冲突
- 增加上游仓库和文档链接

### 推荐提交格式

发起 PR 时，建议附上：

- 项目名称
- 仓库链接
- 简短介绍
- 主要用途
- 适用环境
- 技术特点
- 成熟度说明
- 对应的 README 或文档依据

---

## Roadmap

ClawHome 后续可完善的方向：

- 收录更多生态项目
- 增加上游仓库链接
- 增加机器可读的项目索引
- 增加标签和筛选
- 增加部署示例
- 增加“我该选哪个项目？”的说明
- 增加生态演化时间线

---

## 免责声明

这是一个社区整理性质的导航仓库。

由于生态仍在快速变化，项目的命名、定位、功能和成熟度都可能发生变化。涉及实际部署、选型或生产使用时，请以各项目上游仓库和官方文档为准。

---

## License

MIT
