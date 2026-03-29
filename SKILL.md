# Spreadsheet Table Diagnosis

Use this skill when a spreadsheet task is easier to solve after inspecting the table structure first.

The main goal is to recommend practical next steps for Excel and WPS users, with a bias toward reliable formulas, helper columns, and spreadsheet-native workflows.

## Core Workflow

1. Inspect the input

- Identify whether the user provided headers, sample rows, CSV content, or a direct task description.
- If the table structure is unclear, ask for the smallest amount of extra context needed.

2. Diagnose the table

- Identify likely column types such as IDs, names, dates, status fields, amounts, phone numbers, or free text.
- Look for likely blanks, duplicates, mixed formats, unstable keys, and columns that may need cleanup before formulas are applied.

3. Decide the most practical path

- Prefer simple formulas when they are stable and easy to maintain.
- Prefer Excel and WPS compatible approaches over newer functions with weaker compatibility.
- Prefer helper columns when a single long formula would be fragile.
- Recommend built-in spreadsheet tools when they are a better fit than formulas.

4. Output a clear recommendation

- State what the table appears to contain.
- State what should be done first.
- Recommend the formula or workflow.
- Mention compatibility notes for Excel and WPS.
- Provide a fallback approach if the preferred formula may not work everywhere.

## What This Skill Should Handle Well

- Diagnose messy office tables from headers and sample rows
- Suggest cleanup order for blanks, duplicates, and format issues
- Recommend lookup and matching workflows across sheets
- Suggest summarization and categorization formulas
- Repair common spreadsheet formula mistakes
- Choose between formulas, helper columns, split-text, filters, or pivot tables

## Formula Selection Rules

- Start with the simplest workable formula.
- If a newer function is likely to be unavailable, provide a fallback.
- Prefer `INDEX + MATCH` over `XLOOKUP` when broad compatibility matters.
- Prefer step-by-step text cleanup over nested formulas when readability drops.
- Do not use advanced formulas only to appear clever.

## Compatibility Rules

- Treat Excel and WPS compatibility as an early constraint, not an afterthought.
- Mention when a suggested formula is best for newer Excel only.
- Offer a WPS-friendly or older-Excel-friendly alternative when possible.
- If compatibility is uncertain, recommend a safer helper-column workflow.

## Output Format

Use a structure close to this:

### Diagnosis

- what the table likely contains
- what looks inconsistent or risky

### Recommendation

- what to do first
- which formula or method to use

### Compatibility

- whether it should work in Excel
- whether it should work in WPS
- what fallback to use if needed

### Notes

- where to place the formula
- whether helper columns or built-in tools would be easier

## Boundaries

- Focus on practical spreadsheet handling, not full office automation.
- Do not prioritize styling, chart design, or visual formatting.
- Keep the project centered on diagnosis, cleanup, matching, and summarization.
