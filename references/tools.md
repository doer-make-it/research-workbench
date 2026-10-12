# 工具链配置要点

## Zotero（文献管理）

- 装浏览器插件（Zotero Connector），一键收藏 PDF + 元数据
- 按 课题/方向 建 collection，不按时间
- 定期导出 BibTeX 到 `01_Literature/exports/refs.bib`，Overleaf 引用
- 装 Better BibTeX 插件，引用键自动稳定（`smith2026methane` 格式）
- PDF 重命名规则设为 `作者_年份_标题.pdf`，不存"未命名"

## Python（数据处理）

- 用 venv 隔离环境，不污染系统 Python
- 常用库：pandas / numpy / scipy / matplotlib / openpyxl / originpro
- 脚本头注释：目的、输入、输出、随机种子
- 数据分析脚本存 `03_Data/scripts/`，不散落

## Excel（中间数据）

- 原始数据不动，处理在副本上做
- 一个工作簿一个数据集，sheet 命名清晰（`原始` `清洗` `统计` `图表`）
- 公式留痕，关键计算写注释

## Origin 2024（出版级绘图）

- 通过 `originpro` + COM Automation 驱动自动化绘图
- **单实例模式**：一个 Origin 实例完成所有任务，不重复启动（省 credits），仅在主动要求变更时重启，禁止并行多任务
- 常用图型：K×N 分组柱状图（带误差棒、显著性字母）
- 配色：灰色系为主，避免花哨
- X 轴标签长时旋转
- 输出目录用稳定别名 `数据名_最新/`，覆盖更新，不用时间戳
- 导出 PNG（预览）+ PDF（投稿矢量）

## Overleaf（论文写作）

- Git 同步到本地 `04_Writing/`
- 章节分文件，主文件 `\input`
- 引用走 BibTeX，从 Zotero 导出
- 编译用 XeLaTeX（中文支持）

## Obsidian（知识管理）

- vault 指向 `05_Knowledge/`
- 装 Dataview 插件，自动汇总笔记
- 双链用 `[[概念名]]`，重要概念都建独立笔记
- MOC（Map of Content）聚合每个课题

## Git（版本控制）

- 仓库根在 `project-root/`
- `.gitignore` 排除：大文件（PDF/图片原档视情况）、临时文件、venv
- commit message：`模块-动作-简述`，如 `data-添加品种产量分析脚本`
- 论文 tex 进 Git，大图用 Git LFS 或不进

## 任务管理（Markdown 模板）

- 周计划：`06_Tasks/weekly/YYYY-WW_周计划.md`
- 组会汇报：`06_Tasks/meetings/YYYY-MM-DD_组会汇报.md`
- 日待办：`06_Tasks/todos/YYYY-MM-DD.md`
- 模板见 `references/modules.md` 的"任务管理"章节

## 工具链总原则

- 免费或开源优先，愿意学新工具但不追新
- 单一来源：同一份数据/图表只在一个地方维护，其他地方引用
- 可追溯：文件命名 + 版本号 + Git，任何时候能回到之前状态
