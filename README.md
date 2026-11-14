# Task 2: Test and Improve One Prompt

A 15-case test set for an ecommerce product description prompt, with automatic pass/fail scoring and before/after results.

## Result
| Prompt | Cases passed | Score |
|---|---|---|
| v1 (baseline) | 0 of 15 | 0% |
| v2 (improved) | 15 of 15 | 100% |

## Prompts
- v1: "Write a product description for {product}."
- v2: adds a role, key feature and price as inputs, a 40-60 word limit, a ban on hype words, and a required call to action.

## Pass/fail rules
A case passes only if all 5 rules pass:
1. Length is between 40 and 60 words
2. Mentions the exact product name
3. Mentions the key feature
4. Contains no hype words (best, amazing, perfect, revolutionary, ultimate, incredible)
5. Includes a call to action (order, shop, buy, add to cart, get yours)

## Files
- Task2_Prompt_Test_Results.xlsx
  - Summary: before/after scores, chart and findings
  - Prompts: v1 and v2 text with what changed
  - Rules: editable limits and word lists
  - Run_v1 and Run_v2: 15 test cases with outputs and automatic scoring

## How to reuse
1. Paste your own outputs into column F of a run sheet.
2. Scores recalculate automatically.
3. Edit the word lists on the Rules sheet to change the rules.

## Limitations
Each prompt was run once on one AI model (Claude). Results can vary between runs and tools, so a larger test set would give stronger evidence.

Built as part of the Prompt Engineering (Intermediate) track on Nexlevr.
