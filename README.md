# Serenity Agent

> A QoderWork / AI agent skill that distills Serenity (@aleabitoreddit)'s supply-chain bottleneck investment methodology into a reusable, automated portfolio decision engine.

[中文](#中文) · [English](#english)

---

<a name="english"></a>
## English

### What this is

Serenity Agent is a skill that turns Serenity's "Critical Chokepoint" investment methodology into an automated daily workflow:

1. **Searches** the latest AI semiconductor / photonics / supply-chain news
2. **Analyzes** candidates using the five-step method (chokepoint discovery → first principles → selection signature → rotation logic → narrative hygiene)
3. **Outputs** a structured portfolio decision with position sizing, catalyst calendar, and risk annotations

### The Methodology

Serenity's edge: find the bottleneck in the AI supply chain that the market under-prices, reason from first principles, gate through Buffett-style quality questions, and separate narrative from fundamentals.

**Five-step method:**

| Step | What it does |
|------|-------------|
| 1. Critical chokepoint | Walk the value chain from macro driver to the link where supply can't keep up with demand |
| 2. First principles | Decompose into: demand durability, supply bottleneck, pricing power, capital intensity, geopolitics |
| 3. Selection signature | Small/mid-cap, designed-in, contrarian, dated catalyst |
| 4. Rotation logic | Move UP the supply chain, EARLIER in the cycle, SMALLER/less-covered |
| 5. Narrative hygiene | Quarantine price action, media FUD, and capital flows from quality judgments |

### Install

**QoderWork:**
Copy the skill directory to your skills folder:
```bash
cp -R serenity-agent ~/.qoderwork/skills/
```
Or install the `.skill` package directly in QoderWork.

**Claude Code / Codex:**
```bash
cp -R serenity-agent ~/.claude/skills/      # Claude Code
cp -R serenity-agent ~/.codex/skills/       # Codex
```

### Usage

**Daily portfolio decision:**
> "Run Serenity" / "Serenity 跑一下" / "Serenity daily brief"

The agent will automatically search for today's news, pull prices, and output a portfolio decision.

**Analyze a specific stock:**
> "Analyze $SIVE like Serenity" / "用 Serenity 的方法分析 $SIVE"

**Competition mode:**
> "AI投资竞赛" / "AI stock competition" — outputs formatted for dashboard paste

### Output format

```
## Serenity's Daily Brief — [DATE]

### 市场观察
[AI supply-chain developments]

### 组合决策
| Ticker | 操作 | 目标仓位% | 目标金额$ | 信心 | 理由 |
|--------|------|-----------|-----------|------|------|

### 组合总览 / 催化剂日历 / 风险标注
```

### Automation

Set up a cron/scheduled task to run this skill daily before market close:
- QoderWork: Use the built-in scheduler (Cron skill)
- Claude Code: Use `claude --schedule` or external cron

### File structure

```
serenity-agent/
├── SKILL.md              # Main skill instructions
└── references/
    ├── framework.md      # Full analytical rubric (5 levers, Buffett gate, OSINT heuristics)
    ├── glossary.md       # Jargon definitions (CPO, photonics, financial terms)
    └── exemplars.md      # Worked examples (SIVE, XFAB, SOI, AAOI, Shunsin)
```

### Acknowledgments

- Methodology from [@aleabitoreddit](https://x.com/aleabitoreddit) ("Serenity")'s public archive
- Inspired by [lanfuli/aleabito-serenity-skills](https://github.com/lanfuli/aleabito-serenity-skills) (MIT)
- Not affiliated with Serenity

### Disclaimer

For information tracking and research only. Not investment advice. Do your own due diligence.

### License

[MIT](LICENSE)

---

<a name="中文"></a>
## 中文

### 这是什么

Serenity Agent 是一个 AI 技能，把 Serenity（@aleabitoreddit）的"关键卡点"投资方法论变成一个自动化每日工作流：

1. **搜索** 最新 AI 半导体/光子学/供应链新闻
2. **分析** 候选标的（五步法：卡点发现 → 第一性原理 → 选股签名 → 轮动逻辑 → 叙事卫生）
3. **输出** 结构化持仓决策（仓位、催化剂日历、风险标注）

### 安装

```bash
cp -R serenity-agent ~/.qoderwork/skills/    # QoderWork
cp -R serenity-agent ~/.claude/skills/       # Claude Code
```

### 使用

- **每日持仓决策：** "Run Serenity" / "Serenity 跑一下"
- **分析个股：** "用 Serenity 的方法分析 $X"
- **竞赛模式：** "AI投资竞赛" — 输出格式可直接粘贴到 dashboard

### 免责声明

仅作信息跟踪与研究用途，不构成投资建议。请以自己的尽调为准。

### 许可

[MIT](LICENSE)
