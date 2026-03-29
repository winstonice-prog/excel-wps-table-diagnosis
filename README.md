# excel-wps-table-diagnosis

Read table structure first, then suggest reliable Excel/WPS formulas and cleanup workflows.

一个面向 Excel 和 WPS 的表格诊断与公式建议项目，重点处理脏数据清洗、查找匹配、汇总统计和兼容写法。

## 简介

很多表格问题并不是“缺一个公式”，而是还没先判断清楚这张表真正需要做什么。

这个项目更关注一个更实用的流程：

- 先看表头和样例数据
- 再判断有哪些明显的数据问题
- 然后给出下一步处理建议
- 最后再补上更稳妥的 Excel/WPS 公式或替代做法

它主要面向日常办公表格场景，例如脏数据清洗、两表匹配、汇总统计，以及常见公式问题排查。

## Overview

When working with spreadsheets, the hard part is often not writing a formula, but figuring out what the table needs first.

This project focuses on a simple workflow:

- inspect table structure
- identify likely data issues
- suggest the next processing step
- recommend formulas that are more likely to work in both Excel and WPS
- provide simpler fallback approaches when needed

It is mainly aimed at common office spreadsheet tasks such as cleaning messy columns, matching tables, summarizing data, and fixing common formula problems.

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

- `SKILL.md`: the current skill draft and operating rules
- `examples/table-diagnosis.md`: sample diagnosis workflow
- `examples/sheet-match.md`: sample sheet matching workflow
- `examples/text-cleanup.md`: sample text cleanup workflow
- `examples/README.md`: example index
- `docs/quick-start.md`: short orientation for first-time visitors
- `docs/use-cases.md`: use-case overview
- `docs/roadmap.md`: project direction

## 常见场景

- 先看表，再判断应该先清洗、匹配还是汇总
- 给出兼容 WPS 的公式写法
- 按编号、姓名或其他字段匹配两张表
- 识别空值、重复值和格式不一致的问题
- 建议部门、销售、状态类表格的统计方式
- 排查常见公式报错

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

`Read table structure first, then suggest reliable Excel/WPS formulas and cleanup workflows.`

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
