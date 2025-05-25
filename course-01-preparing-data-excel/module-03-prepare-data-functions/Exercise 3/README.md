
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

**Result in L7:** `$75` (for Region B)

---

### 3. Add Total with Delivery Charge

**Task:**  
In cell `M7`, calculate the sum of the subtotal and delivery charge.

**Formula:**
```excel
=K7+L7
```

**Result in M7:** `$14,250.00`

---

## 📈 Step 3: Autofill Formulas

You copied formulas in `H7`, `L7`, and `M7` down to row `16`.  
Excel showed an "Inconsistent Formula" warning in column `H` due to a different formula structure. This was expected and could be resolved by choosing:

**Option:** `Ignore Error`

---

## 🔢 Step 4: Use `SUMIFS` for Region Totals

Calculate total sales (excluding delivery) for each region.

### Region A (Cell H2)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"A")
```

**Result:** `$40,382.50`

---

### Region B (Cell H3)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"B")
```

**Result:** `$35,100.00`

---

### Region C (Cell H4)

**Formula:**
```excel
=SUMIFS(K7:K16,J7:J16,"C")
```

**Result:** `$21,350.00`

---

## ✅ Conclusion

You’ve now practiced using key Excel formulas:

- `IF` for logical tests
- `IFS` for multiple conditions
- `SUMIFS` for conditional summing

These tools help automate calculations and analyze data based on conditions.

---

🔁 **Review Resources:**

- 📹 *Using the IF Function*
- 📹 *Using Nested IF and IFS*
- 📘 *Reading: AND and OR Functions*

