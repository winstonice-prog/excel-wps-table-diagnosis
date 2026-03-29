# excel-wps-table-diagnosis

Read table structure first, then suggest practical Excel/WPS formulas and cleanup workflows.

先看表结构，再给出更稳妥的 Excel/WPS 处理建议。

## Overview

When working with spreadsheets, the hard part is often not writing a formula, but figuring out what the table needs first.

This project focuses on a simple workflow:

- inspect table structure
- identify likely data issues
- suggest the next processing step
- recommend formulas that are more likely to work in both Excel and WPS
- provide simpler fallback approaches when needed

It is mainly aimed at common office spreadsheet tasks such as cleaning messy columns, matching tables, summarizing data, and fixing common formula problems.

## 中文说明

这个项目更像一个偏实用的表格处理说明书，而不是函数大全。

它主要做三件事：

- 先看表头和样例数据，判断这张表适合先清洗、匹配还是汇总
- 再给出更稳妥的 Excel/WPS 公式或辅助列方案
- 避免一上来就堆很长的公式，优先选择更容易维护的方法

如果一件事更适合用分列、筛选、透视表或辅助列来做，就不强行把所有步骤塞进一个公式里。

## Quick Start

Start with these files:

- `README.md`
- `WORKFLOW.md`
- `examples/README.md`
- `docs/quick-start.md`

Use the current draft in a simple way:

1. Prepare table headers and a few sample rows.
2. Describe the task in plain language.
3. Ask for the safest Excel/WPS-friendly way to handle it.

## 用法

可以直接按下面这种方式使用：

1. 贴出表头和几行样例数据
2. 说明你要做什么，或者直接说“先帮我看这张表”
3. 优先采用兼容 WPS 和 Excel 的稳妥方案

适合的提问方式：

- “先看一下这张表，告诉我应该先处理什么”
- “这两张表按编号怎么匹配，WPS 里也能用”
- “这列日期格式很乱，先怎么清洗比较稳”
- “这个公式为什么会报错，有没有更稳的写法”

## What This Project Focuses On

- Table diagnosis from headers and sample rows
- Formula suggestions for Excel and WPS
- Data cleaning guidance
- Lookup and matching workflows
- Summarization and categorization
- Common formula error troubleshooting

## Why I Made This

A lot of spreadsheet helpers jump straight to formulas.

In real work, that is usually not enough. Before choosing a formula, it helps to know:

- which columns are usable
- whether the data is clean
- whether dates and text formats are consistent
- whether the task is better solved with formulas, helper columns, split text, filters, or a pivot table

This project is built around that step.

## Typical Use Cases

- inspect a table and suggest what to clean first
- recommend a formula that works in WPS
- match two sheets by ID or name
- detect blanks, duplicates, and inconsistent formats
- suggest how to summarize a department, sales, or status table
- troubleshoot common spreadsheet formula errors

## Project Files

- `WORKFLOW.md`: the current workflow notes and handling rules
- `examples/table-diagnosis.md`: sample diagnosis workflow
- `examples/sheet-match.md`: sample sheet matching workflow
- `examples/text-cleanup.md`: sample text cleanup workflow
- `examples/README.md`: example index
- `docs/quick-start.md`: short orientation for first-time visitors
- `docs/use-cases.md`: use-case overview
- `docs/roadmap.md`: project direction
- `CONTRIBUTING.md`: contribution notes
- `CHANGELOG.md`: release history

## Examples

### 1. Diagnose a Messy Table

Input:

`Look at this table and tell me what should be cleaned first.`

Expected output:

- identify blank cells in key columns
- flag duplicate identifiers
- detect mixed date formats
- suggest a practical cleanup order

### 2. Match Two Sheets

Input:

`I need to match Sheet A and Sheet B by customer ID.`

Expected output:

- identify the matching key
- suggest a lookup formula
- provide a WPS-friendly alternative if needed
- recommend a helper-column approach if it is more stable

### 3. Clean a Text Column

Input:

`This column has extra spaces and inconsistent formatting.`

Expected output:

- suggest suitable text functions
- explain whether one formula is enough
- prefer step-by-step cleanup when it is easier to maintain

## Design Principles

- Diagnose before suggesting formulas
- Prefer simple and maintainable solutions
- Consider Excel/WPS compatibility early
- Use helper columns when they make the result more reliable
- Do not force formulas when built-in spreadsheet tools are a better fit

## What This Project Is Not

- not a full office automation toolkit
- not a chart or formatting generator
- not a function encyclopedia with no table context

## Intended Users

- people who work with Excel or WPS regularly
- users who know the task they want to finish, but not the best formula
- beginners who want practical spreadsheet guidance
- anyone dealing with messy office tables

## Repository Notes

- current focus: table diagnosis, formula suggestions, and cleanup workflows
- compatibility is considered early for both Excel and WPS
- this repository is intentionally kept focused on practical spreadsheet tasks

## Roadmap

- better diagnosis from sample data
- stronger Excel/WPS compatibility rules
- formula error repair suggestions
- multi-table merge and reconciliation support
- report-oriented table processing suggestions

## Current Status

This repository is currently in the first public draft stage. The main focus is to make the core positioning, examples, and workflow clear before expanding the project further.

## Suggested Repository Settings

Recommended repository description:

`Read table structure first, then suggest practical Excel/WPS formulas and cleanup workflows.`

Recommended topics:

- `excel`
- `wps`
- `spreadsheet`
- `formula`
- `data-cleaning`
- `table-processing`
- `lookup`
- `productivity`

## License

MIT
