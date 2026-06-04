> ⚠️ **This repo has moved.** Serenity is now one guru inside the unified **[Quant Guru Desk](https://github.com/chuehjen/quant-guru-desk)** — a desk of investing-guru agents you can summon individually or together. This standalone repo is archived and no longer maintained. Please use:
> ```bash
> git clone https://github.com/chuehjen/quant-guru-desk ~/.qoderwork/skills/quant-guru-desk
> ```

---

# Serenity Agent v2

> A QoderWork / AI agent skill that distills Serenity (@aleabitoreddit)'s supply-chain bottleneck investment methodology into a reusable, automated portfolio decision engine.

[中文](#中文) · [English](#english)

---

<a name="english"></a>
## English

### What this is

Serenity Agent v2 is a skill that turns Serenity's "Critical Chokepoint" investment methodology into an automated daily workflow with quantitative scoring:

1. **Searches** the latest AI semiconductor / photonics / supply-chain news
2. **Maps** the 10-layer AI supply chain to identify bottleneck layers
3. **Scores** candidates with an 8-factor chokepoint scorecard (with 8 penalty factors)
4. **Outputs** a structured portfolio decision with quantitative ratings, catalyst calendar, and risk annotations

### The Methodology

Serenity's edge: find the bottleneck in the AI supply chain that the market under-prices, reason from first principles, score quantitatively, gate through Buffett-style quality questions, and separate narrative from fundamentals.

**Nine-step research workflow:**

| Step | What it does |
|------|-------------|
| 1. Set scope | Market, theme, time window |
| 2. System change | Translate narrative into physical constraint |
| 3. Map value chain | 10 layers from raw materials to cloud |
| 4. Find scarce layer | Low suppliers, long qualification, hard expansion |
| 5. Build universe | 20+ candidates, classify by chain position |
| 6. Grade evidence | 4-tier ladder: Strong → Medium → Weak → Needs checking |
| 7. Score & rank | 8 positive factors + 8 penalty factors (0-100) |
| 8. Failure conditions | Substitution, dilution, geopolitics, hype |
| 9. Next research move | Specific filings, metrics, events to watch |

**Three investment phases:**
- Phase 1: Memory (done) → Phase 2: Optical (active) → Phase 3: Silicon Photonics/CPO (emerging)

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
├── SKILL.md                    # Core instructions (9-step workflow + scorecard + modes)
└── references/
    ├── framework.md            # Full analytical rubric + 3-phase cycle
    ├── scoring-system.md       # 8+8 quantitative scorecard with examples
    ├── supply-chain-map.md     # 10-layer AI supply chain + 38 tickers + concentration data
    ├── market-sources.md       # Cross-market data sources (US/A/HK/TW/JP/KR/EU)
    ├── controversies.md        # NINGI report, track record verification, pump-and-dump
    ├── glossary.md             # Jargon definitions (CPO, photonics, financial terms)
    └── exemplars.md            # Worked examples (SIVE, XFAB, SOI, AAOI, Shunsin)
```

### Acknowledgments

- Methodology from [@aleabitoreddit](https://x.com/aleabitoreddit) ("Serenity")'s public archive
- Inspired by [lanfuli/aleabito-serenity-skills](https://github.com/lanfuli/aleabito-serenity-skills) and [muxuuu/serenity-skill](https://github.com/muxuuu/serenity-skill) (MIT)
- Supply chain data from [Epoch AI](https://epoch.ai/data/ai-chip-components) and [semiconstocks.com](https://semiconstocks.com)
- Not affiliated with Serenity

### Disclaimer

For information tracking and research only. Not investment advice. Do your own due diligence.

### License

[MIT](LICENSE)

---

<a name="中文"></a>
## 中文

### 这是什么

Serenity Agent v2 是一个 AI 技能，把 Serenity（@aleabitoreddit）的"关键卡点"投资方法论变成一个自动化每日工作流，含量化评分系统：

1. **搜索** 最新 AI 半导体/光子学/供应链新闻
2. **映射** 10 层 AI 供应链，识别瓶颈层
3. **评分** 候选标的（8 正向因子 + 8 惩罚因子，0-100 分）
4. **输出** 结构化持仓决策（量化评分、催化剂日历、风险标注）

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
