---
name: github-trending-radar
description: Monitor GitHub Trending and turn current popular repositories into a concise Chinese technical radar report. Use when Codex needs to watch GitHub Trending, summarize hot open-source projects, write a technical radar, produce recurring trend briefings, or support an automation that periodically scans public developer trends and turns them into engineering recommendations.
---

# GitHub Trending Radar

## Overview

Observe the current GitHub Trending list, select a small set of notable repositories, and produce a compact Chinese technical radar report for recurring automation runs.
Keep the report decision-oriented. Summarize why each project matters, what signal it may indicate, and what action an engineering team should take next.

## Workflow

1. Gather the current GitHub Trending list from the primary source.
2. Select 3 to 5 repositories that are most worth attention.
3. For each selected repository, explain what it is, why it is currently hot, and what engineering direction it may affect.
4. Produce a fixed-format Markdown radar report in Chinese.
5. Mark uncertainty explicitly when evidence is weak.

## Source Rules

- Prefer GitHub Trending itself as the primary source.
- If the page is partially inaccessible, use another clearly identified public source only to recover missing repository names or descriptions.
- Do not invent star counts, descriptions, release status, company backing, or adoption claims.
- Treat "why it is trending" as an inference unless a source states it directly.
- If the current list cannot be fetched, stop and report the block rather than fabricating a report.

## Selection Rules

Read [references/selection-criteria.md](references/selection-criteria.md) before finalizing the shortlist.

Default shortlist size: 3 to 5 repositories.

Prioritize repositories that signal one of these patterns:
- A new developer workflow or toolchain shift
- A reusable infrastructure or platform pattern
- A strong change in AI, agent, data, frontend, or developer tooling interest
- A project that implies immediate experimentation value for engineers

De-prioritize:
- Joke projects and pure novelty demos with little engineering carryover
- Near-duplicates that express the same signal as a stronger candidate
- Projects with too little information to summarize responsibly

## Reporting Rules

Read [references/report-template.md](references/report-template.md) and follow its section order.

The report must stay compact:
- Title with scan time
- One-sentence conclusion
- 3 to 5 repository notes
- 2 to 3 trend judgments
- Final action labels: `立即试用` / `继续观察` / `先跳过`

For each repository note, include:
- Repository name and link
- What it is
- Why it is hot now
- Likely engineering impact
- Recommended action label

Use plain Chinese. Keep each repository note to 3 to 5 short lines.

## Output Contract

Return only the report unless the user explicitly asks for extra explanation.

If blocked, return a short failure note that includes:
- The source that failed
- What information was missing
- Whether retrying later is likely to work

## Example Triggers

- "监控 GitHub Trending，给我一份技术雷达"
- "总结今天热门开源项目，写成工程决策摘要"
- "每小时扫描 GitHub Trending 并输出中文趋势简报"
- "看看最近 GitHub Trending 有什么值得试用的项目"

## References

- Report structure: [references/report-template.md](references/report-template.md)
- Selection heuristic: [references/selection-criteria.md](references/selection-criteria.md)
