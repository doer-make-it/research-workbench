# 科研工作台 (research-workbench)

> 研究生科研全流程工作平台：文献 → 实验 → 数据 → 论文 → 知识 → 任务，六大模块一条龙。

把散落的科研工作串成可复用工作流，配套七层目录规范、命名规范、工具链配置、组会汇报模板。自用为主、顺便开源。

## 适合谁

- 刚进组、想搭一套能长期用的科研工作流的研究生
- 文件乱、实验记录找不到、组会前突击的人
- 想用 Zotero/Python/Overleaf/Obsidian/Origin 但没串起来的人

## 核心特性

- **七层目录骨架**：`01_Literature` ~ `07_Admin`，固定结构，新人开题直接套
- **命名规范**：`日期_主题_版本`，文件天然可排序、可追溯
- **六大模块工作流**：每模块有明确输入、产出、工具、检查点
- **组会汇报模板**：四要素 + 自检清单，周一早上不慌
- **工具链配置**：Zotero/Python/Origin/Overleaf/Obsidian/Git 关键配置要点

## 快速开始

```bash
# 1. 复制目录骨架到新课题
cp -r assets/folder-template/ my-new-project/

# 2. 按 conventions.md 命名规范开始放文件

# 3. 周一早上用 modules.md 里的组会模板写汇报
```

## 目录结构

```
research-workbench/
├── SKILL.md                    # 工作流主文档（WorkBuddy skill 入口）
├── README.md                   # 本文件
├── LICENSE                     # MIT
├── references/
│   ├── modules.md              # 六大模块详细工作流
│   ├── conventions.md          # 目录与命名规范
│   └── tools.md                # 工具链配置要点
└── assets/
    └── folder-template/        # 可直接套用的空目录骨架
        ├── 01_Literature/
        ├── 02_Experiments/
        ├── 03_Data/
        ├── 04_Writing/
        ├── 05_Knowledge/
        ├── 06_Tasks/
        └── 07_Admin/
```

## 六大模块速览

| 模块 | 输入 | 产出 | 主力工具 |
|---|---|---|---|
| 文献管理 | 论文 PDF | 笔记 + 引用库 | Zotero |
| 实验记录 | 实验过程 | 结构化记录 | Markdown |
| 数据处理 | 原始数据 | 清洗数据 + 图表 | Python + Excel + Origin |
| 论文写作 | 数据 + 文献 | 论文草稿 | Overleaf |
| 知识管理 | 所有产出 | 双链笔记库 | Obsidian |
| 任务管理 | 待办事项 | 周计划 + 组会材料 | Markdown 模板 |

## 与 nature-skills 的区别

`nature-skills` 系列是论文写作各环节的精专工具（润色、绘图、引文、审稿模拟等）。本 skill 管**全局工作流编排**：目录怎么建、文件怎么命名、一周怎么排、组会怎么汇报。两者互补，不冲突。

## 许可证

MIT，自用为主，顺便开源。
