#Exersice 2: Monthly Sales Report - April

## Overview
This README documents the step-by-step process used to analyze and summarize sales data for A2 Mountain Bike Frames in April using Microsoft Excel. The task involved applying core Excel functions such as `SUM`, `AVERAGE`, `COUNT`, `MAX`, and `MIN` to generate meaningful insights from daily sales data. Each step includes not only the formula used, but also the reasoning behind each choice and clarification on common ambiguities.

## File Used
- **Monthly sales report.xlsx**
  - Worksheet: `A2Mountain Bike Frames`
  - Contains daily sales data for the month of April
![image](https://github.com/user-attachments/assets/86b0392f-78fc-4d43-8995-82569c4f1f03)

## Step-by-Step Instructions

### Step 1: Total Revenue Calculation
- **Cell**: `C35`
- **Formula**:  
  ```excel
  =SUM(E4:E33)
  ```
- **Why This Formula?**  
  The `SUM` function is used to add up all revenue values in the range E4 to E33. This gives the total revenue for April.

- **Common Mistake**:  
  AutoSum might suggest `C4:C33` if C35 is selected, which is incorrect because revenue values are in column E.

- **Result**: `$23,059,600` (Accounting format)
![image](https://github.com/user-attachments/assets/fd215bb6-c87a-4ad5-b54e-9599662633da)

---

### Step 2: Total Units Sold
- **Cell**: `C36`
- **Formula**:  
  ```excel
  =SUM(C4:C33)
  ```
- **Why This Formula?**  
  `SUM` adds up all the unit sales in column C (C4:C33). This gives the total number of A2 Mountain Bike Frames sold in April.

- **Result**: `115,298`
![image](https://github.com/user-attachments/assets/045e56e2-1dc0-4e99-9aff-fe650b1ee1ed)

---

### Step 3: Lowest Daily Sales Value
- **Cell**: `C37`
- **Formula**:  
  ```excel
  =MIN(C4:C33)
  ```
- **Why This Formula?**  
  `MIN` finds the smallest value in the specified range. This identifies the day with the lowest unit sales.

- **Result**: `2,560`  
- **Date**: Enter `April 30, 2023` in `D37` (manually identified from the data).
![image](https://github.com/user-attachments/assets/ab6896d4-4694-42b9-89f4-1ed813d146f0)

---

### Step 4: Highest Daily Sales Value
- **Cell**: `C38`
- **Formula**:  
  ```excel
  =MAX(C4:C33)
  ```
- **Why This Formula?**  
  `MAX` retrieves the highest unit sold figure in the range, indicating the day with peak sales.

- **Result**: `4,921`  
- **Date**: Enter `April 16, 2023` in `D38` (manually identified).
![image](https://github.com/user-attachments/assets/6ad147c6-3d5c-4ea0-8d1d-2845427478b6)

---

### Step 5: Count Number of Days in the Month
- **Cell**: `C39`
- **Formula Options**:  
  ```excel
  =COUNT(B4:B33)
  ```  
  or  
  ```excel
  =COUNTA(B4:B33)
  ```

- **Why Use `COUNT` Instead of `COUNTA`?**  
  - `COUNT` counts only numeric values, and since dates in Excel are stored as serial numbers (numeric), it gives an accurate result.
  - `COUNTA` counts all non-empty cells, including text. It works here too, but `COUNT` is cleaner and more precise when you expect only numbers.

- **Why Not Use Fixed Number of Days?**  
  Counting the actual rows allows flexibility for future changes (e.g., if rows are added/removed).

- **Result**: `30`
![image](https://github.com/user-attachments/assets/fb45daea-0ea9-4a4b-9400-13a1c6b4d2ff)

---

### Step 6: Calculate Average Daily Revenue
- **Cell**: `C40`
- **Formula**:  
  ```excel
  =AVERAGE(E4:E33)
  ```
- **Why This Formula?**  
  `AVERAGE` calculates the arithmetic mean of daily revenues, giving insight into daily performance.

- **Result**: `$768,653`  
- **Note**: Automatically formatted as Accounting (currency).
![image](https://github.com/user-attachments/assets/33e0b7f2-f5d4-40a4-9aa2-1240fc74c9cd)

---

## Formatting Tips
- Always check the **Number Format** in the Home ribbon to confirm how values are displayed.
- When using AutoSum or Insert Function, double-check the suggested range and modify if necessary.

