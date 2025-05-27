
# 📊 Excel Exercise: Adding a Data Column Using the IFS Function

## 📝 Overview

In this exercise, I practiced using logical functions in Microsoft Excel by creating formulas to add new data columns and customized totals in a spreadsheet.

### ✅ Objectives

- Create customized totals using the `SUMIFS` formula.
- Use a logical function to test the order value and display the correct discount rate.
- Use the `IFS` function to populate a column with the correct regional delivery charge.



## 📥 Step 1: Download the File

downloaded and opened the Excel workbook `Contoso Bikes.xlsx`.  
It contained one worksheet named `Order Details`, showing details of Contoso Bikes' last order.


## 📊 Step 2: Creating the Calculations

### 1. Apply `IF` Function to Determine Discount Rate

**Task:**  
Create a formula in cell `H7` to check if the subtotal (`G7`) is greater than `$10,000`.

**Formula:**
```excel
=IF(G7>10000,0.1,0)
```
* `Then chnage to the result % form`*
  
**Result:**  
Since `G7` = `$15,750`, the output is `10%`.
*If some values are manually entered on purpose:*

Click the ⚠️ warning icon next to a cell (e.g., `H7`).

Choose "Ignore Error".
![image](https://github.com/user-attachments/assets/fdc3c888-0551-491a-af5a-486bf599742a)


### 2. Apply `IFS` Function to Determine Delivery Charge

**Task:**  
Create a formula in cell `L7` using the `IFS` function to determine delivery charges based on region in `J7`.

**Delivery Charges (use absolute references):**

- Region A → `$D$2`
- Region B → `$D$3`
- Region C → `$D$4`

**Formula:**
```excel
=IFS(J7="A",$D$2, J7="B",$D$3, J7="C",$D$4, TRUE, 0)
```
### ✅ Formula 1 (Correct Syntax)
```excel
=IFS(J7="A", $D$2, J7="B", $D$3, J7="C", $D$4, TRUE, 0)
```
- Straight quotes (`"A"`)
- Uppercase `TRUE` (standard boolean)
- Readable spacing



### ❌ Formula 2 (Incorrect Syntax)
```excel
=IFS(J7=”A”,$D$2,J7=”B”,$D$3,J7=”C”,$D$4,True,0)
```
- Curly quotes (`”A”`) → Causes `#NAME?` error
- Lowercase `True` (non-standard)
- No spacing



### 🔧 Fixes Needed
- Replace smart quotes with `"`.
- Use `TRUE` instead of `True`.

---

### ❗ Why It Matters
- Excel treats smart quotes as text → Errors.
- `TRUE/FALSE` are reserved; `True/False` may fail or behave inconsistently.



### ✅ Final Corrected Version
```excel
=IFS(J7="A", $D$2, J7="B", $D$3, J7="C", $D$4, TRUE, 0)
```

**Result in L7:** `$75` (for Region B)

![image](https://github.com/user-attachments/assets/cf5576c5-9309-447c-91dc-d1494ca29ccc)


### 3. Add Total with Delivery Charge

**Task:**  
In cell `M7`, calculate the sum of the subtotal and delivery charge.

**Formula:**
```excel
=K7+L7
```

**Result in M7:** `$14,250.00`

![image](https://github.com/user-attachments/assets/75d55b38-ebbb-4d5a-bc66-962572a8f0f2)


## 📈 Step 3: Autofill Formulas

You copied formulas in `H7`, `L7`, and `M7` down to row `16`.  
Excel showed an "Inconsistent Formula" warning in column `H` due to a different formula structure. This was expected and could be resolved by choosing:

**Option:** `Ignore Error`



## 🔢 Step 4: Use `SUMIFS` for Region Totals

Calculate total sales (excluding delivery) for each region.

### Region A (Cell H2)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"A")
```

# ✅ SUMIFS Formula Correction and Explanation

## 📝 Problem Description

In the exercise, you were asked to create a `SUMIFS` formula in cell **H2** that calculates total **sales (excluding delivery)** for a specific region (e.g., Region B). However, the formula given was:

```excel
=SUMIFS(J7:J16, "B", K7:K16)
```

This caused an incorrect result or a #SPILL! or ##### error after formatting it as currency.

❌ Issues in the Original Formula  
**Incorrect Argument Order**  
The SUMIFS function syntax is:

```excel
=SUMIFS(sum_range, criteria_range, criteria)
```

But the original formula reversed the sum_range and criteria_range.

**Smart Quotes Used**  
Excel does not accept curly quotes like “B” or ”B”. It needs straight quotes: "B".

##### Error in Cell  
After applying the currency format, Excel displayed ##### — this is not a formula error. It means the column is too narrow to show the full number.

✅ Corrected Formula  
To calculate the total sales in K7:K16 where the region in J7:J16 is "B", the correct formula is:

```excel
=SUMIFS(K7:K16, J7:J16, "B")
```

💡 Explanation  
- K7:K16 is the range of sales data (values to be summed).  
- J7:J16 is the region data (criteria range).  
- "B" is the condition to match Region B.  
- Quotes must be straight ("B") for Excel to read it correctly.

🔧 Fix for ##### Display  
If the result shows as ##### after formatting to Currency:

👉 Widen the column: Drag the column border to make it wider.

✅ This fixes the display, and the value (e.g., $33,382.50) will appear properly.

✅ Final Notes  
- Always use the correct argument order in SUMIFS:  
  `=SUMIFS(sum_range, criteria_range, criteria)`  
- Avoid using smart quotes — use straight quotes for strings.  
- If you see #####, it usually means the cell is too narrow — not that the formula is wrong.

**Result:** `$40,382.50`


### Region B (Cell H3)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"B")
```

**Result:** `$35,100.00`



### Region C (Cell H4)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"C")
```

**Result:** `$21,350.00`

![image](https://github.com/user-attachments/assets/caea6851-0302-4d0a-8eab-5de291b2f52b)



## ✅ Conclusion

We’ve now practiced using key Excel formulas:

- `IF` for logical tests
- `IFS` for multiple conditions
- `SUMIFS` for conditional summing

These tools help automate calculations and analyze data based on conditions.


🔁 **Review Resources:**

- 📹 *Using the IF Function*
- 📹 *Using Nested IF and IFS*
- 📘 *Reading: AND and OR Functions*

