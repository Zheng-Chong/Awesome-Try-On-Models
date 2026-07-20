# Project Handoff

更新时间：2026-07-20
当前分支：main
当前目标：维护 Awesome-Try-On-Models 的最新开源试穿模型条目

## 项目状态

- 仓库当前维护 `README.md` 中的 `Image-based Models`、`Video-based Models`、`3D-based Models` 三类条目，按日期倒序排列。
- 新增条目需要优先使用论文链接，并在可验证存在官方代码仓库时使用 GitHub Star 徽章格式补充代码链接。
- 本次维护按“论文或官方页面可核实，且官方 GitHub/Hugging Face 已公开实际代码或官方权重”筛选；纯 README 占位、Coming Soon、纯项目页和纯数据集不收录。

## 最近任务

### 目标
- 执行每周维护，筛选并补充截至 2026-07-20 符合条件的开源试穿模型。

### 已完成
- 检查工作区干净状态并执行 `git pull --ff-only`，确认本地与 `origin/main` 同步。
- 检索近期 image、video、3D try-on 候选，排除仅有项目页、README 占位、纯数据集或未公开代码/权重的条目。
- 在 `README.md` 的 `Image-based Models` 中新增 `RefTon` 条目。
- 创建仓库级 `HADNOFF.md`，作为后续自动维护入口。

### 关键决策
- `RefTon` 被收录，因为其论文、官方 GitHub 仓库、官方 Hugging Face 模型页和权重发布均可核实，且仓库包含实际训练/推理代码；README 日期按 arXiv 首次提交时间 `2025-11-02` 记录。
- `CtrlVTON`、`Vanast`、`TryOnCrafter`、`TAMF-VTON`、`MOFA-VTON` 等候选未收录，因为截至 2026-07-20 仍缺少公开实际代码或官方权重，或仅提供项目页/README 占位。
- `Dress-ED`、`MV-Fashion`、`Garments2Look` 等以数据集/benchmark 为主的仓库未作为新增模型条目录入。

### 涉及范围
- `README.md`：补充符合条件的 image-based model 条目并保持日期倒序。
- `HADNOFF.md`：记录本次筛选标准、验证结论和下一会话入口。

### 验证
- `git pull --ff-only`：通过，仓库已同步。
- 链接核验：已核对 `RefTon` 的 arXiv、GitHub 和 Hugging Face 官方页面可访问且内容匹配。
- GPU 运行验证：未运行：本机无 GPU 环境。

## 剩余事项与风险

- 尚未执行提交、推送、Notion 回写前的最终 `git diff --check` 与新增链接命令行复核。
- 后续维护时仍需继续关注近期仅发布项目页/README 的候选是否补齐正式代码或官方权重。

## 下一会话

1. 先检查 `git status --short` 与 `git pull --ff-only`，确认仓库仍干净且与远端同步。
2. 重点复查最近未收录候选是否已补齐官方代码或权重，再决定是否继续更新 `README.md`。

## 最近历史

- 2026-07-20：完成一次周维护，新增 `RefTon` 条目并建立仓库交接文件。
