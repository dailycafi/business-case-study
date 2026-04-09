# Teaching Case Development Skill for Claude

A comprehensive skill for developing business school teaching cases — from topic evaluation through writing, classroom testing, to journal submission.

## What It Does

Guides case authors through a 6-stage iterative workflow:

1. **Direction Anchoring** — three-line parallel research (company, industry, novelty)
2. **Information Exhaustion** — 5-dimension topic evaluation matrix, interview outline design
3. **Information Collection** — interview transcript analysis, topic crystallization
4. **Writing-Crystallization Loop** — iterative case body + teaching note development with "triple delivery" per round (manuscript, alignment check, next step)
5. **Classroom Testing** — feedback integration
6. **Submission / Revision** — rubric benchmarking, reviewer response

## Key Features

- **5-dimension topic evaluation matrix**: novelty, teaching value, theoretical richness, information availability, discussion scope
- **Rubric-aligned quality checks**: case body (4x25 points) and teaching note (25+15+35+25 points)
- **Writing style enforcement**: narrative (HBS+WSJ), forbidden expression detection, citation standards
- **Teaching note design**: What→Why→How logic chain, Bloom's taxonomy, "升维" (elevation) methodology
- **Trigger word system**: natural language triggers for each stage transition

## Install

### Claude Code

```bash
git clone https://github.com/dailycafi/business-case-study.git ~/.claude/skills/business-case-study
```

### Claude.ai

Download as ZIP, upload via Settings > Capabilities > Skills.

## Usage

Natural language triggers:

- "新案例：[公司名]，[课程方向]，一手/二手"
- "采访回来了" + paste transcript
- "开始写" or share a draft
- "选题定了：[description]"
- "准备投稿"
- "审稿意见回来了" + paste reviewer comments

## Structure

```
business-case-study/
├── SKILL.md                              # Core workflow + triggers
└── references/
    ├── topic-evaluation.md               # 5-dimension matrix, 3-line research
    ├── rubric-case-body.md               # Case body scoring (4x25 pts)
    ├── rubric-teaching-note.md           # Teaching note scoring (25+15+35+25)
    └── writing-style.md                  # Narrative style, forbidden expressions
```

## License

MIT
