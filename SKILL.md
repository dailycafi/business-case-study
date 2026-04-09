---
name: business-case-study
description: Structured business case analysis in the Harvard Business School (HBS) tradition with strategic frameworks (SWOT, Porter's Five Forces, PESTLE, BCG Matrix, Value Chain), alternatives evaluation, and actionable recommendations. Use when user mentions case study analysis, MBA assignments, strategic analysis of a company, competitive analysis homework, SWOT analysis, or asks to apply business frameworks. Also triggers when users paste business case text or upload case PDFs for analysis. Supports Chinese and English output.
metadata:
  author: cafi
  version: 1.0.0
  category: education
  tags: [MBA, strategy, case-study, business-analysis]
---

# Business Case Study Analyzer

Produce rigorous, insight-driven case analyses grounded in case facts — the kind that earns top marks at HBS, Wharton, or INSEAD. Every claim must reference case data, not generic platitudes.

For detailed framework guidance (SWOT deep-dive, Porter's rating scales, financial ratio cheat sheet), consult `references/frameworks.md`.

## Step 0: Gather the Case Material

- **PDF or file provided:** Read it fully before analyzing.
- **Text pasted:** Use it directly.
- **Verbal description:** Ask for: company name, industry, time period, central decision/dilemma, and any professor-specified frameworks.
- **Well-known case by name** (e.g., "Southwest Airlines", "Cola Wars"): Draw on knowledge but flag: "Note: my analysis is based on the commonly taught version of this case. Your version may differ in specific exhibits or data."

Proceed only when you have enough material to ground the analysis in facts.

## Step 1: Case Overview

2-3 paragraphs covering:
- **Company and Context** — protagonist, industry, time period
- **Central Issue** — what decision must be made, why now, what's at stake
- **Scope** — geographic, business unit, time horizon boundaries

Goal: someone who hasn't read the case understands the situation after this section.

## Step 2: Situation Analysis

Select 2-3 frameworks that illuminate this specific case. Do not apply every framework mechanically.

**Quick selection guide:**

| If the case is about... | Use... |
|------------------------|--------|
| Overall strategy | SWOT + one other |
| Industry attractiveness | Porter's Five Forces |
| External environment shifts | PESTLE |
| Cost/operations | Value Chain Analysis |
| Portfolio of businesses | BCG Matrix |
| Growth direction | Ansoff Matrix |
| Sustainable advantage | VRIO |
| Competitor response | Game Theory |

For deep framework guidance, read `references/frameworks.md`.

**Critical quality rule:** Every framework point must cite case facts. Quantify where possible.

**Example — B-level vs. A-level SWOT:**

B-level: "Strength: strong brand."

A-level: "The brand commands a 15% price premium (Exhibit 3), but this premium eroded from 22% over five years, suggesting the moat is narrowing. 40% of COGS is tied to one supplier (Exhibit 5), creating supplier power risk."

## Step 3: Key Issues

Distill 3-5 strategic issues from Step 2, ranked by impact and urgency. For each:
- What specifically is the problem?
- Why does it matter? (quantify if possible)
- How does it connect to the other issues?

## Step 4: Strategic Alternatives

Present 3 distinct alternatives. "Do nothing / status quo" counts if viable.

For each alternative, include:
- **Description** — what specifically the company would do
- **Pros** — concrete benefits with supporting logic
- **Cons** — concrete risks with supporting logic
- **Financial Impact** — order-of-magnitude estimate if data supports it
- **Feasibility** — can this be executed with available resources?

Alternatives must be genuinely different strategic directions. Three versions of "expand internationally" = one alternative with sub-options, not three.

## Step 5: Recommendation

Pick one alternative (or phased combination) and defend it:
- **What** — the recommendation in 1-2 sentences
- **Why** — strategic logic referencing Step 2 frameworks
- **How** — implementation roadmap with phases, milestones, timeline
- **Risk Mitigation** — what could go wrong and how to hedge
- **Success Metrics** — KPIs, financial targets, milestones

The recommendation should feel inevitable from the preceding analysis.

## Step 6: Conclusion and Takeaways

2-3 paragraphs: What strategic principles does this case illustrate? What can other companies learn? What broader trends does it connect to?

## Output Format

```
# [Company Name] Case Analysis

## 1. Case Overview
## 2. Situation Analysis
### 2.1 [Framework 1]
### 2.2 [Framework 2]
## 3. Key Issues
## 4. Strategic Alternatives
### Alternative 1: [Name]
### Alternative 2: [Name]
### Alternative 3: [Name]
## 5. Recommendation
## 6. Conclusion and Takeaways
```

## Language Convention

- User writes Chinese: body in Chinese, terms in English, headers bilingual (e.g., "案例概述 (Case Overview)")
- User writes English: all English
- Mixed: default to Chinese body with English terms

## Examples

**Example 1: Directed analysis request**

User: "帮我分析 Southwest Airlines 的案例，教授要求用 Porter's Five Forces 和 SWOT"

Action: Use Porter's Five Forces and SWOT as specified. Suggest additional framework only if it clearly adds value. Output in Chinese with English terms.

**Example 2: Open-ended analysis**

User: "Analyze Netflix's decision to split streaming and DVD in 2011"

Action: Choose frameworks yourself (likely SWOT + Game Theory for competitor dynamics). Output in English. Focus on the specific decision point.

**Example 3: Case PDF uploaded**

User: [uploads case PDF] "写一篇 case analysis，3000字"

Action: Read PDF fully. Select frameworks based on case content. Respect the word limit — compress situation analysis, keep alternatives tight. Output in Chinese.

## Adaptation

- **User specifies frameworks:** Use those, even if you'd choose differently.
- **Page/word limit:** Adjust depth accordingly.
- **Presentation format:** Use bullet-heavy structure instead of essay.
- **Class discussion prep (not written assignment):** Focus on 2-3 provocative discussion questions rather than definitive recommendation.

## Common Issues

**Analysis feels generic:**
- Go back to case exhibits and data. Every SWOT bullet should cite a specific fact.
- Ask: "Could this sentence apply to any company?" If yes, rewrite with specifics.

**Alternatives are too similar:**
- Test: could you collapse them into one? If yes, they're variations, not alternatives.
- Try: one conservative option, one aggressive, one transformative.

**Recommendation feels arbitrary:**
- Check: does the recommendation address the #1 key issue from Step 3?
- Check: does it leverage the top strength and mitigate the top threat from Step 2?

## Performance Notes

- Take your time to do this thoroughly
- Quality is more important than speed
- Do not skip the quality checks above
