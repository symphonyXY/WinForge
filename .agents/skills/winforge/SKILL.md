---
name: winforge
description: 专用于 Windows 桌面应用的设计与 Vibe Coding 开发。1:1 复刻最新 Apple / iOS 液态玻璃与 OriginOS 光影原子两大核心审美体系（支持局部混搭），精细打磨背景、按键、按钮与物理弹簧动效；针对模糊需求用通俗语言反问并给建议；智能选型并严格保证 .exe 安装包在新电脑上零额外下载、装完即用；强约束项目文件夹分区、模块化代码规范与安全清理。
---

# WinForge — Windows 桌面应用设计与工程指南

本 Skill 面向**无开发基础、采用 Vibe Coding 方式打造高颜值 Windows 桌面软件**的用户。AI 执行任何任务时，始终遵守五条铁律：

1. **说人话，先对齐再动手**：禁止堆砌晦涩技术术语。遇到模糊需求，先用大白话追问 2–4 个最关键的问题并附带推荐方案；确认后先跑出一个能点开体验的最小雏形，再陪用户逐步精修。
2. **审美贵精不贵多，细节 1:1 拉满**：只使用本仓沉淀的 **Apple / 最新 iOS 液态玻璃** 与 **最新 OriginOS 空间光影原子** 两大视觉体系（二选一或按部位混搭）。对背景材质、按键/按钮手感、圆角比例、悬浮胶囊与物理弹簧动效做像素级打磨，彻底杜绝廉价 AI 模板味。
3. **新电脑装完即用，绝对零额外下载**：交付的 Windows `.exe` 必须把运行环境、字体、图标和依赖全部离线内置。**严禁**在线联网安装器，**严禁**弹窗要求用户去装 `.NET`、`VC++`、`Python`、`Node.js` 或联网下组件。默认打包为离线一键安装版 `Setup.exe`，用户要求时再切换或加打绿色免安装版。
4. **文件夹永远清爽，代码模块化好维护**：强制分区存放源码、素材、文档和打包产物，禁止根目录散落临时文件、测试脚本、日志或 `_old`/`_bak` 备份；禁止把所有代码塞进超大单文件；删除已有文件前必须先列清单请示；大改前主动提醒做 Git 版本存档。
5. **诚实交付，眼见为实**：不虚报未测试的功能或打包结果。每次修改后用通俗语言说明改了什么、怎么打开体验，以及当前是否已实际打包/验证。

---

## 按需阅读地图

只读取与当前阶段相关的手册，不要一次全塞进上下文：

| 当前阶段 / 用户意图 | 必读手册 | 同步参考样板间 |
|---|---|---|
| 新想法起步、需求模糊、拆解任务 | [需求引导与 Vibe Coding 协作](references/workflow-and-vibe-coding.md) | — |
| 选技术栈、确定打包方案、解决“换电脑打不开” | [架构选型与离线打包铁律](references/architecture-and-packaging.md) | — |
| 采用 **Apple / 最新 iOS & macOS** 液态玻璃风格 | [Apple / iOS 液态玻璃体系](references/style-apple-ios.md) + [通用交互细节与避坑红线](references/motion-and-craft-guardrails.md) | [Apple 交互样板间](showcases/apple-liquid-glass.html) |
| 采用 **最新 OriginOS** 光影与原子交互风格 | [OriginOS 光影原子体系](references/style-originos.md) + [通用交互细节与避坑红线](references/motion-and-craft-guardrails.md) | [OriginOS 交互样板间](showcases/originos-atomic-light.html) |
| 两大风格按部位混搭 / 精修按钮、按键、背景与动效 | 两份风格手册 + [通用交互细节与避坑红线](references/motion-and-craft-guardrails.md) | 两份交互样板间 |
| 搭建目录、重构旧代码、整理垃圾文件、Git 存档 | [文件夹管理与开发规范](references/project-hygiene-and-standards.md) | — |

---

## 标准工作流（新建 Windows 软件）

1. **短问对齐（1 轮搞定）**：读取 `workflow-and-vibe-coding.md`。若需求不够明确，用大白话问 2–4 个关键问题（核心功能、选 Apple 还是 OriginOS、浅/深外观偏好、架构推荐），每题给出直接可拍板的推荐选项。
2. **拍板架构与骨架**：读取 `architecture-and-packaging.md` 与 `project-hygiene-and-standards.md`。按需求推荐最稳的架构（通常带高颜值界面优先 Electron，追求极小体积且主攻 Win11 选 Tauri，纯系统小工具选 C# 自包含），建好分区清晰的干净目录。
3. **1:1 复刻视觉与交互雏形**：读取选定的风格手册、`motion-and-craft-guardrails.md` 及对应 `showcases/*.html` 样板间代码，先交付**能直接打开、能点主流程、颜值在线**的最小可运行版本。
4. **边看边精修 + 安全存档**：根据用户反馈逐项微调视觉与功能；每次完成满意阶段或要做大改版前，主动提醒做一次 Git 提交留好“后悔药”。
5. **离线打包与收尾自检**：按 `architecture-and-packaging.md` 打包为离线一键安装版 `Setup.exe`（输出集中放到 `release/`），核对新电脑防翻车清单，清理本次产生的临时文件，交付清晰中文说明。

## 已有项目维护 / 颜值升级

1. 先查看目录结构与 Git 状态，绝不覆盖用户未提交的改动，不无故更换技术栈。
2. 如果项目文件夹已混乱，先只读盘点并列出整理清单，获用户同意后再归类或清理。
3. 视觉升级时严格对照选定的 Apple 或 OriginOS 手册与避坑红线，把样板间里的材质、圆角、按钮按压与弹簧动效真正落进真实组件。
