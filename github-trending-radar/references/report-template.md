# GitHub Trending 技术雷达报告模板

按下面结构输出，不要额外扩展长篇前言。

```md
# GitHub Trending 技术雷达 | {{scan_time}}

一句话结论：{{today_main_signal}}

## 热门项目观察

### 1. {{owner}}/{{repo}}
链接：{{repo_url}}
它是什么：{{one_sentence_summary}}
为什么现在热门：{{reason_or_inference}}
工程影响：{{engineering_impact}}
建议动作：{{立即试用|继续观察|先跳过}}

### 2. {{owner}}/{{repo}}
链接：{{repo_url}}
它是什么：{{one_sentence_summary}}
为什么现在热门：{{reason_or_inference}}
工程影响：{{engineering_impact}}
建议动作：{{立即试用|继续观察|先跳过}}

## 趋势判断
- {{trend_1}}
- {{trend_2}}
- {{trend_3_optional}}

## 工程建议
- 现在关注：{{one actionable follow-up}}
- 保持观察：{{one trend to watch}}
- 暂不跟进：{{one low-signal area or noisy item}}
```

约束：
- 整篇保持紧凑，适合高频自动化运行。
- 如果只有 3 个项目值得写，就只写 3 个，不要为了凑数硬写。
- `为什么现在热门` 可以是推断，但要避免过度确定。
