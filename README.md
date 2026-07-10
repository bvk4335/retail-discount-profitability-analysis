# Quantitative Analysis of Retail Pricing & Discount Strategy

## Problem Statement:
Discounting is one of the easiest levers a retail business can pull to boost sales — and one of the easiest ways to quietly bleed money. Revenue can look great on paper while every extra sale is actually costing the company money. It's a trap a lot of retail and D2C companies have fallen into (Doodhwala and Shuttl are two examples that come to mind).

This project starts from one simple question:

Is this company's discounting actually helping it grow — or is it slowly draining its profits?

## Project_Objectives:
- Understand how sales and revenue are performing across product categories, regions, and sales channels.
  
- Check whether discounting is actually helping profit, or burning the profits.
  
- Estimate how sensitive customers really are to price changes (elasticity).
  
- Identify the exact point where a discount stops being profitable and starts causing losses.
  
- Simulate what happens to profit if discounting is brought back under control.

## Approach:

- Started with exploratory analysis across categories, regions, sales reps, and channels to see where revenue and profit    diverge.
- Explored core profitability metrics (profit, margin, break-even discount) — see METRICS.md for exact formulas.
  
- Checked correlation between discounting and sales/quantity to see if discounts were actually driving demand.
  
- Estimated price elasticity to test how price-sensitive customers really are.
  
- Ran a break-even discount analysis to find the exact point where discounting turns unprofitable.
  
- Simulated capped-discount pricing to measure how much profit could be recovered.

## Key Findings:

- Revenue was healthy across every region and category — but profit margins were negative almost everywhere, meaning growth wasn't translating into actual money made.

- 60.4% of transactions were sold at a discount higher than the product's break-even point — meaning the company was guaranteed to lose money on the majority of its sales.

- Discounting showed no meaningful positive relationship with sales volume or revenue — customers weren't buying more because of the discount.

- Price elasticity was statistically weak (R² ~0.01), showing customers weren't reacting to price the way the discount strategy assumed.

- Electronics was the only category priced within a sustainable range — every other category was regularly sold below cost.

- Capping discounts at the break-even level would have significantly improved total profit, without needing any drop in sales volume.

- A multivariate check confirmed discount is the only statistically significant driver of profit — category, region, and channel showed no independent effect once discount was accounted for, ruling out those as root causes

## Final_Recommendations:
- Set a maximum discount cap for each product category, based on its break-even point.
  
- Track sales rep performance on margin, not just revenue.
  
- Build in regular pricing reviews so discounts don't drift upward unchecked.
  
- Treat unit economics (profit per sale) as a core metric alongside revenue, not an afterthought.
