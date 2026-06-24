# Cyrus Skills

[![License: MIT](https://img.shields.io/badge/License-MIT-b3854d.svg)](LICENSE)
[![Skills](https://img.shields.io/badge/skills-2_published-b3854d.svg)](#-skills)
[![RedSkill](https://img.shields.io/badge/小红书-RedSkill-ff2442.svg)](https://www.xiaohongshu.com)
[![Made with Claude Code](https://img.shields.io/badge/Made_with-Claude_Code-5A67D8.svg)](https://claude.com/claude-code)

**中文** | [English](#english)

我是 Cyrus，文科生，不会写代码，但用 AI 交付了几个商业级项目。

这里是我**日常真实在用**的 Agent Skills 合集——不是理论整理，每一条规则都来自真实项目的教训（56 份计划文档、带证据的验收记录、踩过的真实事故）。逐期公开。

---

## 📦 Skills

| Skill | 一句话 | 状态 |
|---|---|---|
| **[AI 编码 12 步工作流](./cyrus-coding-12steps/SKILL.md)**<br>`cyrus-coding-12steps` | vibe coding 不翻车指南。6 个核心步人人必做，6 个进阶步项目变大再开。逼 AI 把「能用」的证据拿出来，而不是说一句「完成了」 | ✅ 第 1 期已公开 |
| **[AI Mirror — 用真实数据蒸馏你自己](./ai-mirror/SKILL.md)**<br>`ai-mirror` | 比 MBTI 准 100 倍。把聊天记录、录音、行为数据喂给 AI，6+1 层框架蒸馏出你的决策逻辑、情绪模式、关系姿态、行为盲区。杀手锏：对比"你说的 vs 你做的"，找出你自己都不知道的说-做差距 | ✅ 第 2 期已公开 |
| 自媒体 Skills<br>`cyrus-media-skills` | 选题挖掘 / 写稿 / 过审 / 数据复盘 / 发布追踪 | 🔜 第 3 期打磨中 |

### 12 步速览（cyrus-coding-12steps）

| # | 步骤 | 一句话 | 级别 |
|---|------|--------|------|
| 1 | 沟通规则 | AI 先说人话解释，再给命令 | 🟤 核心 |
| 2 | 需求四件套 | 做什么、怎么验收，写清楚再动手；说不清就让 AI 采访你 | 🟤 核心 |
| 3 | 定义怎么算过 | 检查先于代码，跑通什么才算完成 | 🟤 核心 |
| 4 | 分支隔离 | 不直接动 main，搞砸随时退回 | ⚪ 进阶 |
| 5 | 小步提交推远端 | 推上云端才算保住 | ⚪ 进阶 |
| 6 | 验证方法论 | 要证据不要「完成了」；Playwright 自动验收 + 截图存证 | 🟤 核心 |
| 7 | 上下文管理 | 纠错两次就重开，治鬼打墙 | 🟤 核心 |
| 8 | VERIFY 验收交接 | 要测什么，写进文档不靠记 | ⚪ 进阶 |
| 9 | PLAN 治理 | 大活先写计划，用户批了才动手 | ⚪ 进阶 |
| 10 | 安全基线 | 密钥不进代码，依赖先查真假 | ⚪ 进阶 |
| 11 | Review 门禁 | 合并上线前再过一遍 | ⚪ 进阶 |
| 12 | 交付契约 | 交活必给五样：文件、命令、证据、风险、回滚 | 🟤 核心 |

## 🚀 安装

把 `SKILL.md` 放进你的 Agent skills 目录即可：

```bash
# AI Mirror（自我认知蒸馏）
mkdir -p ~/.claude/skills/ai-mirror
curl -o ~/.claude/skills/ai-mirror/SKILL.md \
  https://raw.githubusercontent.com/cyrus-tt/cyrus-skills/main/ai-mirror/SKILL.md

# AI 编码 12 步工作流
mkdir -p ~/.claude/skills/cyrus-coding-12steps
curl -o ~/.claude/skills/cyrus-coding-12steps/SKILL.md \
  https://raw.githubusercontent.com/cyrus-tt/cyrus-skills/main/cyrus-coding-12steps/SKILL.md
```

- **Cursor**：内容并入 `.cursorrules` 或项目规则文件
- **小红书 RedSkill**：在我的笔记里点 skill 组件，复制口令粘给你的 AI 一键安装

> ⚠️ 安全提醒：口令/脚本安装等于让 AI 执行远程指令，只装可信来源的 skill。

## 💡 为什么有这套东西

AI 写代码很快，但「写完」不等于「能用」。

我交付商业项目时踩过的坑：AI 说全做完了，上 Staging 一测有个接口压根没开发；回滚脚本写着「开始回滚」实际只打印了四个字。这些坑后来全变成了步骤。

这套 skill 的设计原则：

- **分级**：核心步人人必做，进阶步带触发条件，小脚本不堆仪式
- **证据驱动**：完成的定义 = 证据，不是 git commit
- **小白友好**：worktree、CORS、smoke test 全部一句话人话解释

---

<a name="english"></a>
## English

I'm Cyrus — a liberal-arts grad who can't write code, but has shipped several commercial-grade projects with AI.

This is a collection of Agent Skills I **actually use daily**. Every rule comes from real project lessons (56 plan documents, evidence-backed verification records, real incidents) — not theory. Published episode by episode.

**Skills:**

- **[ai-mirror](./ai-mirror/SKILL.md)** — Distill yourself from real data. Feed your chat logs, recordings, and behavioral data to AI — get back your decision patterns, emotional triggers, relationship dynamics, and blind spots. The killer feature: Layer 7 "Behavior Audit" compares what you *say* you do vs what you *actually* do. No personality test can do that.
- **[cyrus-coding-12steps](./cyrus-coding-12steps/SKILL.md)** — A 12-step AI coding workflow that keeps vibe coding from falling apart. 6 core steps for everyone, 6 advanced steps that activate as your project grows. Forces the AI to show *evidence* that things work, instead of just saying "done".
- **cyrus-media-skills** — Content creation workflow (topic mining / writing / review / analytics). Coming soon.

**Install** — drop `SKILL.md` into your agent's skills directory (`~/.claude/skills/` for Claude Code, `~/.agents/skills/` for Codex and friends, or merge into `.cursorrules` for Cursor).

> ⚠️ Installing a skill means letting your AI execute remote instructions. Only install from sources you trust.

## License

[MIT](LICENSE)
