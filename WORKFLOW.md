# Spreadsheet Table Diagnosis Workflow

This document records the main handling rules used in this repository.

The goal is simple: look at the table first, then choose a practical way to clean, match, summarize, or troubleshoot it in Excel and WPS.

## Core Workflow

1. Inspect the input

- Identify whether the input contains headers, sample rows, CSV content, or a direct task description.
- If the table structure is still unclear, ask for the smallest amount of extra context needed.

2. Diagnose the table

- Identify likely column types such as IDs, names, dates, status fields, amounts, phone numbers, or free text.
- Look for blanks, duplicates, mixed formats, unstable keys, and columns that should be cleaned before formulas are applied.

3. Choose the most practical path

- Prefer simple formulas when they are stable and easy to maintain.
- Prefer Excel and WPS compatible approaches over newer functions with weaker compatibility.
- Prefer helper columns when a single long formula would be fragile.
- Recommend built-in spreadsheet tools when they are a better fit than formulas.

4. Present a clear recommendation

- State what the table appears to contain.
- State what should be done first.
- Recommend the formula or workflow.
- Mention compatibility notes for Excel and WPS.
- Provide a fallback approach if the preferred formula may not work everywhere.

## What This Repository Should Handle Well

- messy office tables built from headers and sample rows
- cleanup order for blanks, duplicates, and format issues
- lookup and matching workflows across sheets
- summarization and categorization formulas
- common spreadsheet formula mistakes
- choosing between formulas, helper columns, split-text, filters, or pivot tables

## Formula Selection Rules

- Start with the simplest workable formula.
- If a newer function is likely to be unavailable, provide a fallback.
- Prefer `INDEX + MATCH` over `XLOOKUP` when broad compatibility matters.
- Prefer step-by-step text cleanup over nested formulas when readability drops.
- Do not use advanced formulas only to appear clever.

## Compatibility Rules

- Treat Excel and WPS compatibility as an early constraint.
- Mention when a suggested formula is best for newer Excel only.
- Offer a WPS-friendly or older-Excel-friendly alternative when possible.
- If compatibility is uncertain, recommend a safer helper-column workflow.

## Output Shape

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
