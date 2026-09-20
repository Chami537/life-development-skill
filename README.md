# 人生发展 Skill

**结合一个人的真实处境，帮他理清困惑、比较选择，并找到眼下能做的下一步。**

基于 [《高性价比人生指南》](https://github.com/eternity4719/HowToLiveBetter)提炼的 AI 答疑技能，适用于支持 `SKILL.md` 的智能助手。显示名称为 **人生发展**，调用名为 **`life-development`**。

它把指南中的判断方法用于对话：先了解对方想保住什么、有哪些限制，再分别考虑健康、金钱、时间与精力、权利，以及关系和个人意义。需要具体依据时，再查阅随技能附带的资料。

## 可以用来聊什么

- **学习与工作**：读书还是工作、学什么技能、转行、辞职、失业后的安排。
- **钱与生活保障**：消费、储蓄、现金流、保险、租房、救助和待遇的查询路径。
- **关系与家庭**：恋爱、催婚、婚姻分工、照料家人、育儿与个人边界。
- **习惯与状态**：睡眠、精力、拖延、信息过载、压力与生活节奏。
- **困难处境**：重大变故后先处理什么，怎样找支持、留材料、走办事流程。

例如：

> 用人生发展 skill 帮我分析：我想辞职转行，但只有两个月生活费，应该怎么安排？

> 父母一直催婚，我暂时不想结。我想维护自己的选择，也不想一直和他们吵。

> 我每天下班都很累，还想学点东西。能不能帮我找一个能坚持下来的起点？

## 它如何答疑

1. **理解处境**：区分事实、感受和推测，只补问会影响判断的信息。
2. **按需找依据**：从相关章节读取完整条目，包括备注、适用条件和争议。
3. **比较可行路径**：分别说明成本、收益、风险、退出条件，以及不行动的代价。
4. **给出下一步**：通常先提出一到三个具体动作；不确定时，优先设计能退出的小尝试。

对方只想倾诉或理解一件事时，技能不会强行做人生规划。否定一种做法时，会尽量给原本合理的需求提供替代路径，例如如何表达感谢、验证转行方向或处理家庭期待。

## 安装到 Codex

需要先安装 Git。把整个仓库克隆到 Codex 的技能目录，**文件夹名使用 `life-development`**。

### Windows PowerShell

```powershell
$skillRoot = if ($env:CODEX_HOME) { Join-Path $env:CODEX_HOME 'skills' } else { Join-Path $HOME '.codex\skills' }
New-Item -ItemType Directory -Path $skillRoot -Force | Out-Null
git clone https://github.com/Chami537/life-development-skill.git (Join-Path $skillRoot 'life-development')
```

### macOS / Linux

```bash
skill_root="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$skill_root"
git clone https://github.com/Chami537/life-development-skill.git "$skill_root/life-development"
```

如果目标文件夹已经存在，先检查已有内容，不要覆盖自己的修改。安装后新开一个会话；如果技能列表尚未刷新，重启客户端后再查看。

其他支持技能的助手，可以按其安装方式导入整个文件夹。技能正文与资料不依赖专用服务；`agents/openai.yaml` 是 Codex 的显示元数据。只有核实现行政策、研究等信息时才需要可用的联网能力。

## 使用

在 Codex 对话中输入：

```text
$life-development

我目前的处境是……
我最想解决的是……
我担心或不能承受的是……
请帮我比较可行选择，给出眼下的下一步。
```

也可以直接说“用人生发展技能帮我分析……”。不必先填完整问卷，助手会按问题补问必要背景。默认允许自动选择该技能，是否实际触发取决于宿主助手。

## 文件结构

```text
life-development/
├── SKILL.md                  答疑方法、判断原则与回答方式
├── agents/openai.yaml        名称、简介与默认调用提示
└── references/
    ├── topics.md             按问题找章节，记录资料版本
    ├── evidence.md           证据解释、时效核对与适用边界
    └── guide/
        ├── README.md         原指南导读
        ├── LICENSE           原指南许可
        ├── book/             32 章、552 条建议
        └── docs/             4 篇专题长文、引用对照、75 份核实记录
```

资料按需读取，不应每次把整本书全部放入上下文。原指南导读中部分图片、网站与发行文件指向上游内容，完整阅读体验可访问[原项目](https://github.com/eternity4719/HowToLiveBetter)。

## 来源、证据与边界

本项目是基于原指南制作的独立技能，并非原作者官方发布的技能。

| 项目 | 当前版本 |
| --- | --- |
| 资料来源 | [eternity4719/HowToLiveBetter](https://github.com/eternity4719/HowToLiveBetter) |
| 快照日期 | 2026-09-20 |
| 上游提交 | [`74c39f36d0f5e4fda17b0e48ff8066c966c7794c`](https://github.com/eternity4719/HowToLiveBetter/tree/74c39f36d0f5e4fda17b0e48ff8066c966c7794c) |
| 更新方式 | 随仓库版本人工更新，不自动追踪上游 |

技能明确区分**指南记载、当前核实的事实、基于个人处境的推断**。引用链接和作者的 A/B/C 标签不等于本次已经独立验证；观察性相关不能直接转成对个人的因果承诺。资料里的政策金额、资格、期限和医学建议，仍需结合当前地区、人群和官方来源核对。

不同种类的收益不强行折算成一个分数，无法量化的兴趣、情感和承诺也有价值。原书对受益人的排序不被用作人的价值高低，最后的选择仍由当事人决定。

这套技能提供信息梳理与决策支持，不代替诊断、处方或针对具体案件的专业意见。遇到眼前的严重危险，先帮助求助；对于普通迷茫和压力，不自动升级为危机。

## 更新与改进

以克隆方式安装后，可在技能目录执行：

```bash
git pull --ff-only
```

有本地修改时先保留修改并检查差异。维护资料快照时，同步更新本页与 [`references/topics.md`](references/topics.md) 的日期、提交和统计信息；不要只替换某个数字却丢掉来源、备注或适用条件。

欢迎通过 [Issues](https://github.com/Chami537/life-development-skill/issues) 提交答疑中的具体问题或来源纠错。请隐去姓名、联系方式、病历身份信息等可识别个人的内容。改进技能应针对实际出现的问题，避免不断增加对所有问题都强制执行的流程。

## 许可

本仓库采用 [Unlicense](LICENSE)。附带的原指南文本同样采用 Unlicense，其[原许可文件](references/guide/LICENSE)保留在资料目录内；引用论文与外部网页仍遵循各自的权利和使用条件。
