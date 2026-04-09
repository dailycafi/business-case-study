# Business Case Study Skill for Claude

Structured business case analysis in the Harvard Business School (HBS) tradition. Produces rigorous, insight-driven case analyses with strategic frameworks, alternatives evaluation, and actionable recommendations.

## What It Does

- Reads business case materials (PDF, pasted text, or verbal descriptions)
- Applies 2-3 relevant strategic frameworks (SWOT, Porter's Five Forces, PESTLE, BCG Matrix, Value Chain, etc.)
- Identifies key strategic issues ranked by impact
- Evaluates 3 distinct alternatives with pros/cons/feasibility
- Delivers a defended recommendation with implementation roadmap
- Supports both Chinese and English output

## Install

### Claude Code

Place the skill folder in your Claude Code skills directory:

```bash
git clone https://github.com/dailycafi/business-case-study.git ~/.claude/skills/business-case-study
```

### Claude.ai

1. Download this repo as a ZIP
2. Open Claude.ai > Settings > Capabilities > Skills
3. Upload the ZIP file
4. Enable the skill

## Usage

Just describe your case study task:

- "帮我分析 Southwest Airlines 的案例，教授要求用 Porter's Five Forces 和 SWOT"
- "Analyze Netflix's decision to split streaming and DVD in 2011"
- Upload a case PDF and ask: "写一篇 case analysis"

The skill automatically activates when it detects case study analysis requests.

## Structure

```
business-case-study/
├── SKILL.md                    # Core workflow (~150 lines)
├── references/
│   └── frameworks.md           # Detailed framework guide (SWOT, Porter's, PESTLE, financial ratios)
└── README.md                   # This file (for humans, not loaded by Claude)
```

## License

MIT
