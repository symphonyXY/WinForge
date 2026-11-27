# WinForge

专用于 **Windows 桌面软件设计与 Vibe Coding 开发** 的个人审美与工程 Skill 仓库。

不贪多、不堆砌花哨模板，只专注于把每一款做出来的 Windows 软件打磨到**高颜值、好手感、新电脑装完直接用、文件夹永远干净利落**。

---

## 核心特色

1. **双核心顶级审美（1:1 复刻 + 支持局部混搭）**
   - **Apple / 最新 iOS & macOS 液态玻璃**：四层光学液态玻璃、连续嵌套圆角、一体化融合顶栏 + 精修右上角 Windows 窗口按钮、灵动岛胶囊、丝滑弹簧回弹。
   - **最新 OriginOS 空间光影与原子交互**：自然弥散环境光影、模块化原子卡片（支持点击原位放大与沿原路弹回）、原子岛快捷面板、厚胶囊阻尼推杆与 Q 弹物理手感。
2. **对零基础 Vibe Coding 极度友好**
   - 遇到模糊想法时，AI 先用大白话反问 2–4 个最关键的问题并附推荐方案，绝不甩一堆听不懂的程序员黑话。
   - 先快速做出**能点开体验的高颜值最小雏形**，再陪你边看边精修。
3. **新电脑装完 `.exe` 直接用，零额外下载**
   - 写死离线打包铁律：严禁在线安装器，严禁弹窗提示安装 `.NET`、`VC++`、`Python` 或联网下载运行库；字体、图标与运行环境全部离线内嵌。
   - 默认交付离线一键安装版 `Setup.exe`（支持选安装路径、建桌面快捷方式、干净卸载），按需切换或加打绿色免安装版。
4. **文件夹洁癖 + 模块化代码 + Git 安全网**
   - 强制源码、素材、文档、打包产物分门别类，严禁根目录乱堆临时脚本、日志和 `_old`/`_bak` 备份；严禁把所有代码塞进超大单文件；删除已有文件必先列清单请示；大改前主动提醒做 Git 存档。

---

## 先看效果：双击打开两份离线样板间

下面两份交互样板间**无需联网、无需安装任何环境**，直接用 Edge 或 Chrome 浏览器双击就能打开试玩，亲自体验按钮按压、开关、滑块、灵动岛/原子岛、原位放大与浅深切换：

- **Apple / iOS 液态玻璃样板间**：[.agents/skills/winforge/showcases/apple-liquid-glass.html](.agents/skills/winforge/showcases/apple-liquid-glass.html)
- **OriginOS 光影原子样板间**：[.agents/skills/winforge/showcases/originos-atomic-light.html](.agents/skills/winforge/showcases/originos-atomic-light.html)

> 以后你觉得某个圆角、玻璃通透度或回弹手感还可以更好，直接打开样板间指出哪里要调，我同步改好样板间和规则手册，后面做的所有软件就会自动沿用你调好的新审美。

---

## 怎么用这套 Skill

- **在 Antigravity 中使用**：直接打开本仓库，或把整个 `.agents/skills/winforge/` 文件夹复制到你的新软件项目根目录的 `.agents/skills/` 下（或复制到用户全局 skills 目录），直接用大白话说出你想做的软件即可。
- **在 Codex / Cursor / Claude Code 等兼容工具中使用**：同样整目录放入 `.agents/skills/winforge/`，对话时直接描述需求，或显式说明“使用 winforge Skill”。

### 常用开场白示例（直接复制就能用）

```text
用 winforge 帮我做一个 Windows 桌面番茄钟，我想要 Apple 液态玻璃风格，先按大白话问清楚细节并推荐合适的架构。
```

```text
用 winforge 帮我做一个本地壁纸和截图整理工具，想要 OriginOS 光影原子风，卡片点开能原位放大预览，最后打包成新电脑装完就能直接用的 Setup.exe。
```

```text
用 winforge 检查并重构我现在这个软件的界面和文件夹：按 Apple 液态玻璃 + OriginOS 原子岛的混搭风格重新精修按钮和动效，把根目录乱七八糟的文件整理干净（删除旧文件前先列清单给我确认）。
```

---

## 仓库目录一览

```text
WinForge/
├── README.md                                            # 本说明文档
├── LICENSE                                              # MIT 开源许可
└── .agents/skills/winforge/                             # 完整可独立拷贝的 Skill 包
    ├── SKILL.md                                         # 总指挥入口与行为铁律
    ├── references/
    │   ├── workflow-and-vibe-coding.md                  # 模糊需求反问与 Vibe Coding 协作节奏
    │   ├── style-apple-ios.md                           # Apple / 最新 iOS 液态玻璃 1:1 手册
    │   ├── style-originos.md                            # 最新 OriginOS 光影原子 1:1 手册
    │   ├── motion-and-craft-guardrails.md               # 背景/按键/按钮/动效细节与去 AI 味红线
    │   ├── architecture-and-packaging.md                # 智能架构选型与离线 Setup.exe 打包铁律
    │   └── project-hygiene-and-standards.md             # 文件夹分区、模块化代码与 Git 安全网
    └── showcases/
        ├── apple-liquid-glass.html                      # Apple 液态玻璃交互样板间
        └── originos-atomic-light.html                   # OriginOS 光影原子交互样板间
```

---

## 以后怎么继续补充和扩展

- **微调审美细节**：直接修改对应样板间（`showcases/*.html`）和对应风格手册（`references/style-*.md`）。
- **新增第 3 种风格**：在 `references/` 新建一份 `style-xxx.md` 和对应样板间，并在 `SKILL.md` 的「按需阅读地图」里加上一行即可。
- **补充个人开发习惯**：直接追加到 `references/project-hygiene-and-standards.md` 或 `references/workflow-and-vibe-coding.md`。
