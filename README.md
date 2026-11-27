# WinForge

专用于 **Windows 桌面软件设计与 Vibe Coding 开发** 的个人审美与工程 Skill 仓库。

不贪多、不堆砌花哨模板，只专注于把每一款做出来的 Windows 软件打磨到**高颜值、好手感、新电脑装完直接用、文件夹永远干净利落**。

---

## 核心特色

1. **双核心顶级审美与跨平台范式（1:1 复刻 + 支持局部混搭）**
   - **Apple OS 27 全生态液态玻璃**（融合 iOS 27 / macOS 27 Golden Gate / iPadOS 27 / watchOS 27 / visionOS 27）：均匀折射与高对比度精修、**Ultraclear ↔ Fully Tinted 无级透度滑块**、macOS 27 通边液态玻璃侧栏与统一工具条、watchOS 27 Smart Stack 迷你情景挂件与动态高频网格、visionOS 27 三分区控制中心与悬停聚焦展开、灵动岛胶囊与丝滑弹簧回弹。
   - **OriginOS 7 空间光影与原子交互**：**Dynamic Translucent Material 三档动态半透明材质**（Realistic 拟真 / Natural 自然 / Soft 柔和）、**Dynamic Glow 光随手走实时交互光晕**、Fluid Motion 水滴拉伸与速度感知 Q 弹弹簧、模块化原子卡片原位放大、**Origin Workbench 多任务卡片工作台**、**Origin Island + Snap & Go 主动情景原子岛**、夜间护眼 4.0（以及受控可选的 Glint / Wiggle 轻趣味风味）。
   - **按需加载的桌面 AI 与情景交互范式**：仅在做带 AI/智能建议的软件时启用，覆盖 Spotlight Ask AI、随处润色改写、情景建议胶囊、多模板摘要与高亮视图、AI 舒适阅读模式与透明可审计的代理隐私活动日志。
2. **对零基础 Vibe Coding 极度友好**
   - 遇到模糊想法时，AI 先用大白话反问 2–4 个最关键的问题并附推荐方案，绝不甩一堆听不懂的程序员黑话。
   - 先快速做出**能点开体验的高颜值最小雏形**，再陪你边看边精修。
3. **新电脑装完 `.exe` 直接用，零额外下载**
   - 写死离线打包铁律：严禁在线安装器，严禁弹窗提示安装 `.NET`、`VC++`、`Python` 或联网下载运行库；字体、图标与运行环境全部离线内嵌。
   - 默认交付离线一键安装版 `Setup.exe`（支持选安装路径、建桌面快捷方式、干净卸载），按需切换或加打绿色免安装版。
4. **文件夹洁癖 + 模块化代码 + Git 安全网**
   - 强制源码、素材、文档、打包产物分门别类，严禁根目录乱堆临时脚本、日志和 `_old`/`_bak` 备份；严禁把所有代码塞进超大单文件；删除已有文件前必须先列清单请示；大改前主动提醒做 Git 存档。

---

## 先看效果：双击打开两份离线样板间

下面两份交互样板间**无需联网、无需安装任何环境**，直接用 Edge 或 Chrome 浏览器双击就能打开试玩，亲自体验无级液态玻璃、三档动态材质、通边侧栏、Smart Stack、三分区控制中心、Dynamic Glow、Origin Workbench、Snap & Go 原子岛与原位放大：

- **Apple OS 27 全生态液态玻璃样板间**：[.agents/skills/winforge/showcases/apple-liquid-glass.html](.agents/skills/winforge/showcases/apple-liquid-glass.html)
- **OriginOS 7 光影原子样板间**：[.agents/skills/winforge/showcases/originos-atomic-light.html](.agents/skills/winforge/showcases/originos-atomic-light.html)

> 以后你觉得某个圆角、玻璃通透度、三档材质或回弹手感还可以更好，直接打开样板间指出哪里要调，让 AI 同步改好样板间和规则手册，后面做的所有软件就会自动沿用你调好的新审美。

---

## 怎么用这套 Skill

- **在 Antigravity 中使用**：直接打开本仓库，或把整个 `.agents/skills/winforge/` 文件夹复制到你的新软件项目根目录的 `.agents/skills/` 下（或复制到用户全局 skills 目录），直接用大白话说出你想做的软件即可。
- **在 Codex / Cursor / Claude Code 等兼容工具中使用**：同样整目录放入 `.agents/skills/winforge/`，对话时直接描述需求，或显式说明“使用 winforge Skill”。

---

## 实战示例（直接复制改两个字就能用）

### 示例 1：6 大高频场景开场白模板

#### 场景 A · Apple OS 27 全生态液态玻璃新软件（效率 / 笔记 / AI 助手 / 悬浮挂件）
```text
用 winforge 帮我做一个 Windows 桌面番茄钟与 AI 待办助手。
风格选 Apple OS 27 液态玻璃：主窗口用 macOS 通边液态侧栏，支持无级玻璃透度调节和 Ctrl+K 呼出 Ask AI；迷你模式切成 watchOS Smart Stack 情景小挂件。先用大白话跟我对齐 3 个关键细节并推荐架构，确认后先出最小雏形。
```

#### 场景 B · OriginOS 7 光影原子新软件（多任务看板 / 文件整理 / 文档阅读）
```text
用 winforge 帮我做一个本地 PDF 与截图整理工作台，想要 OriginOS 7 光影原子风：
支持 Realistic/Natural/Soft 三档动态材质和夜间护眼 4.0，主界面用原子卡片原位放大 + Origin Workbench 多任务切换，拖入截图时用顶部原子岛 Snap & Go 给一键归档建议。最后打包成新电脑装完即用的离线 Setup.exe。
```

#### 场景 C · Apple OS 27 + OriginOS 7 局部混搭
```text
用 winforge 帮我做一个桌面快捷启动与剪贴板历史软件。
视觉上混搭一下：整体窗口用 Apple macOS 27 通边液态玻璃侧栏和统一工具条，任务切换用 OriginOS 7 Workbench 卡片与 Dynamic Glow 随手光晕，控制面板参考 visionOS 三分区控制中心。
```

#### 场景 D · 给已有旧软件“去 AI 味 + 颜值大升级”
```text
用 winforge 帮我给当前这个 Windows 软件做一次颜值和交互精修：
去掉原来的紫粉渐变、Emoji 图标和死板弹窗，按 Apple OS 27 液态玻璃规范重做一体化无割裂顶栏、通边侧栏、圆润窗口按钮、按钮 6 种状态和物理弹簧动效。动手前先帮我做一次 Git 存档留底。
```

#### 场景 E · 打包“新电脑装完即用”离线安装包
```text
用 winforge 帮我把现在的软件打包成 Windows 离线一键安装版 Setup.exe，放到 release/ 文件夹里。
要求：在刚买的新电脑上断网安装也能直接双击打开，绝对不能弹窗让装运行库或连外网下字体；如果方便，顺便再告诉我怎么切出绿色免安装版。
```

#### 场景 F · 整理混乱文件夹 & 安全清理垃圾
```text
用 winforge 帮我盘点并整理一下当前项目的文件夹：
把源码、素材、文档和打包产物按规范分区，把超大的单文件按职责拆清爽。注意：清理任何原本就存在的旧文件前，必须先用大白话列清单给我确认，别私自删文件。
```

---

### 示例 2：普通 AI 写法 vs WinForge 1:1 复刻效果对比

| 细节部位 | 普通 AI 容易写出来的“廉价感” | 使用 WinForge 后的真实落地效果 |
|---|---|---|
| **窗口与导航** | 上面一条死板纯白/纯黑 Windows 原生标题栏，侧栏和内容硬线割裂 | 一体化无边框融合顶栏 + macOS 27 通边液态侧栏或悬浮水滴胶囊 + 精修右上角圆润窗口按钮 |
| **背景与玻璃** | 高饱和紫粉霓虹渐变，或一坨发灰浑浊、看不清字的毛玻璃 | 低饱和柔和环境光 + Apple OS 27 无级透度液态玻璃 / OriginOS 7 三档动态材质 + 夜间护眼 4.0（正文对比度 ≥ 4.5:1） |
| **图标与字体** | 满屏 `🚀✨⚙️📁` 系统 Emoji，换台电脑字体回退成丑陋宋体 | 统一圆润线宽的精细矢量 SVG 图标 + 随包离线内置的高颜值字体，任何新电脑观感一致 |
| **按钮与动效** | 鼠标点下去毫无反应，弹窗生硬闪现，动画播到一半打断就瞬移 | 完整 6 态按钮 + Dynamic Glow 随手光晕 + 速度感知物理弹簧回弹 + 原子卡 FLIP 原位放大与无缝打断 |
| **AI 与情景交互** | 硬塞一个花哨发光聊天框，自动改用户文件也不留记录 | 隐形融入的 Spotlight Ask AI、随处改写、Snap & Go 情景岛、AI 舒适阅读模式与透明中文隐私活动日志 |
| **软件打包** | 发给朋友一双击就弹窗“请先安装 .NET / WebView2 / Python” | 默认离线一键安装 `Setup.exe`，字体、图标与运行环境全内置，断网新电脑装完即用 |
| **项目文件夹** | 根目录堆满 `test2.js`、`backup_old/`、`1.png` 和 2000 行巨型文件 | 严格分区（源码 / 素材 / 文档 / `release/` 成品），模块化拆分 + 中文备注 + Git 存档 |

---

## 仓库目录一览

```text
WinForge/
├── README.md                                            # 本说明文档与实战示例
├── LICENSE                                              # MIT 开源许可
└── .agents/skills/winforge/                             # 完整可独立拷贝的 Skill 包
    ├── SKILL.md                                         # 总指挥入口、行为铁律与按需阅读地图
    ├── references/
    │   ├── workflow-and-vibe-coding.md                  # 模糊需求反问与 Vibe Coding 协作节奏
    │   ├── style-apple-ios.md                           # Apple OS 27 全生态液态玻璃 1:1 手册
    │   ├── style-originos.md                            # OriginOS 7 空间光影与原子交互 1:1 手册
    │   ├── motion-and-craft-guardrails.md               # 背景/按键/按钮/动效细节与去 AI 味红线
    │   ├── ai-and-contextual-patterns.md                # 【按需】桌面 AI 与情景交互范式手册
    │   ├── architecture-and-packaging.md                # 智能架构选型与离线 Setup.exe 打包铁律
    │   └── project-hygiene-and-standards.md             # 文件夹分区、模块化代码与 Git 安全网
    └── showcases/
        ├── apple-liquid-glass.html                      # Apple OS 27 全生态液态玻璃交互样板间
        └── originos-atomic-light.html                   # OriginOS 7 光影原子交互样板间
```

---

## 以后怎么继续补充和扩展

- **微调审美细节**：直接修改对应样板间（`showcases/*.html`）和对应风格手册（`references/style-*.md`）。
- **新增第 3 种风格**：在 `references/` 新建一份 `style-xxx.md` 和对应样板间，并在 `SKILL.md` 的「按需阅读地图」里加上一行即可。
- **补充个人开发习惯**：直接追加到 `references/project-hygiene-and-standards.md` 或 `references/workflow-and-vibe-coding.md`。
