# Metrics & Formulas

This file documents every metric engineered for the analysis, and the formula behind each one.

## 1. Effective Unit Price
The price the customer actually paid after discount.

Effective_Unit_Price = Unit_Price * (1 - Discount)

## 2. Calculated Revenue
Revenue recalculated from effective price, used as a validation check against the raw Sales_Amount column.

Calculated_Revenue = Effective_Unit_Price * Quantity_Sold

## 3. Profit (per transaction)
Profit = (Effective_Unit_Price - Unit_Cost) * Quantity_Sold

## 4. Margin %
Profit as a share of revenue — lets categories/regions be compared fairly regardless of size.

Margin_% = (Profit / Calculated_Revenue) * 100

## 5. Profit without Discount
What profit would have looked like at full price. Used as a baseline to isolate the cost of discounting.

Profit_no_Discount = (Unit_Price - Unit_Cost) * Quantity_Sold

## 6. Discount Impact
How much profit was given up because of the discount.

Discount_Impact = Profit_no_Discount - Profit

## 7. Profit per Discount Loss
How much profit is generated for every unit of profit given up to discounting — a ratio to gauge overall discount efficiency.

Profit_per_Discount_Loss = Total_Profit / Total_Discount_Impact

## 8. Break-Even Discount
The maximum discount a product can absorb before it starts selling at a loss.

Max_Discount = 1 - (Unit_Cost / Unit_Price)
