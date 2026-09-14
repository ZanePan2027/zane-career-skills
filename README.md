# 走出象牙塔

简体中文 | [English](README.en.md)

> 把你做过的事，整理成简历、作品集和清楚的求职表达。

[![Version](https://img.shields.io/badge/version-v1.0.0-2563EB.svg?style=flat-square)](VERSION.md)
[![License](https://img.shields.io/badge/license-MIT-16A34A.svg?style=flat-square)](LICENSE)

**AI 求职工具箱。给正在从校园走向职场，也在毕业后重新认识自己的年轻人。**

从课程、社团、实习和工作经历中找到能说明能力的材料，对照岗位形成求职方向，完成多语言简历、作品集和面试表达。经历逐渐丰富时，同一套方法也可以继续用于跳槽和职业转向。

**适用于 Claude Code、Codex，以及其他支持 Agent Skills 的工具。免费开源。**

[快速开始](#快速开始) · [它解决什么](#它解决什么) · [能力一览](#能力一览) · [安装](#安装) · [使用方法](#使用方法)

![从经历到求职表达](docs/career-assets-flow.zh-CN.svg)

## 它解决什么

从一段真实经历开始，找到与目标岗位有关的能力和表达。

| 想推进的事 | 工具箱帮你推进到 |
| --- | --- |
| 整理课程、社团、实习或第一份工作 | 找出本人做过的动作、留下的作品和可支持的能力 |
| 比较求职方向，或毕业后重新定位 | 对照岗位任务与自己的经历，形成候选方向和具体尝试 |
| 完成中文、英文或其他语言简历 | 按招聘市场组织内容、结构与版式，生成可编辑稿和交付文件 |
| 展示项目和作品 | 安排简历、网站与深读案例的分工，构建作品集 |
| 准备自我介绍、项目追问和面试 | 用同一份真实经历准备回答，逐轮练习并改进表达 |
| 整理团队项目与前雇主材料 | 写清本人贡献，选择适合公开或面试展开的信息 |
| 更新多种语言与载体 | 把事实变化同步到简历、网页、案例和面试材料 |

## 快速开始

### 1. 安装

```bash
npx -y skills add ZanePan2027/zane-career-skills -g --all
```

### 2. 直接告诉 Agent 你的处境

```text
请使用 zane-career-assets。
我正在准备第一份工作，做过一个课程项目，也负责过社团活动报名和签到。
这是我的项目报告和经历说明，请帮我找出能写进简历的内容，
并对照这两个岗位，看看各自需要突出哪些经历。
```

也可以直接提出当前要完成的事：

```text
请使用 zane-career-assets。我毕业两年，想比较继续做运营和转向品牌策划，
这是我做过的工作与两份岗位说明，请帮我比较。

请使用 zane-career-resume-builder，把这些经历整理成申请产品实习的英文简历。

请使用 zane-career-assets，围绕这份简历和岗位说明，和我逐轮模拟项目面试。

请使用 zane-career-portfolio-website-design，根据这些项目做一个作品集网站。
```

## 它怎样工作

从你提供的经历中整理事实与证据，再对照岗位决定要突出什么、用什么载体表达。简历、作品集、投递消息与面试回答共同使用这些材料；你纠正一个事实后，相应内容会一起调整。

例如，一次社团活动可以提供组织与执行的线索。工具箱会区分你的具体动作、团队的工作和活动规模，写成清楚的简历条目，再把同一经历展开成面试时可以讲明白的过程。

## 能力一览

| 工作目标 | 主要入口 | 常见产出 |
| --- | --- | --- |
| 整理经历、比较方向、准备面试 | `zane-career-assets` | 经历证据、岗位比较、回答稿与逐轮演练 |
| 完成整套求职材料 | `zane-career-portfolio-builder` | 简历、作品集、案例与投递入口 |
| 创建或本地化简历 | `zane-career-resume-builder` | 内容、版式、可编辑源与 PDF |
| 设计作品集的阅读顺序 | `zane-career-portfolio-architecture` | 首页、案例深读与作品索引 |
| 构建作品集网站 | `zane-career-portfolio-website-design` | 视觉设计、响应式页面与实现文件 |
| 写清项目案例 | `zane-career-case-editor-zh`、`zane-evidence-weighted-case-storytelling` | 判断、动作、结果与本人贡献 |
| 处理前雇主材料 | `zane-former-employer-data-redactor` | 适合公开、脱敏或面试展开的内容 |
| 写投递第一句话 | `zane-career-application-greeting` | 对应岗位与语言的短招呼语 |
| 检查交付文件 | `zane-portfolio-multi-format-qa` | 网页、PDF、Word、二维码与链接检查 |
| 使用视觉参考 | `zane-design-reference-to-prompt` | 设计方向与实现要求 |

日常从 `zane-career-assets` 进入。想做特定任务时，直接调用对应入口。详细说明见 [能力目录](docs/skill-inventory.md)。

## 安装

### 推荐：安装全部 Skills

```bash
npx -y skills add ZanePan2027/zane-career-skills -g --all
```

也可以直接告诉 Agent：

```text
请从 https://github.com/ZanePan2027/zane-career-skills 安装全部 Skills，
然后使用 zane-career-assets，帮我处理这件事：……
```

安装后按工具要求重载 Skills。项目级安装与更新见 [安装说明](docs/install.md)。

## 使用方法

提供这次的求职目标和手边材料：一段经历、旧简历、课程报告、作品或岗位说明。工具箱会从当前任务开始，按需要整理和制作。

- **整理经历时**，讲清你做过什么，并带上能帮助还原过程的材料。
- **制作求职材料时**，说明岗位、招聘市场、语言及想拿到的文件。
- **准备面试时**，提供本次使用的简历和岗位，让 AI 帮你写回答或逐轮练习。
- **收到新反馈时**，带回招聘者的问题、修改意见或自己的事实纠正，继续调整相关材料。

成果保存在你选择的项目位置。需要下次继续时，让 Agent 保存当前材料和暂停点。

## 来源与许可证

这套方法来自简历、双语作品集、项目案例和求职交付中的持续实践，结合按岗位取材、跨载体一致性和实际反馈完善。

设计参考见 [来源说明](docs/provenance.md)。本仓库采用 [MIT License](LICENSE)。

作者：Zane
