
# 📊Module 1 Exercise 4: Calculating Profit and Margin

## 📁 Overview
This exis designed to guide me through basic financial calculations in Microsoft Excel, focusing on profit margins, total costs, revenues, and more. i use Excel formulas to compute important values, learn about how these calculations work from an economic perspective, and explore key business concepts like cost of goods sold (COGS), markup pricing, and profit margins.

---

## ✅ Steps to Perform the Calculation

### 🔽 Step 1: Download the File
1. First, download the Excel workbook named **Revenue figures.xlsx**.
2. The workbook will contain data such as **Wholesale Cost**, **Quantity Purchased**, **Shipping Cost**, and **Quantity Sold**, but columns **G**, **H**, **I**, **J**, **L**, and **M** will initially be blank.
![image](https://github.com/user-attachments/assets/dff6f54f-667e-4425-8965-bf8ca0708131)

---

### ✏️ Step 2: Apply the Formulas

#### 2.1 ➕ **Purchase Cost (G4)**
To calculate the **Purchase Cost**, we multiply the **Wholesale Cost** (cell E4) by the **Quantity Purchased** (cell F4). This gives us the total cost for purchasing the stock.

- **Formula**:  
  ```excel
  =E4*F4
  ```
- **Economic Concept**:  
  This calculation is related to **Cost of Goods Sold (COGS)**, which represents the direct costs of producing the goods that a company sells. It’s important because knowing the cost helps businesses price their products correctly.

- **Expected Result**: `$1,010,216.69`
![image](https://github.com/user-attachments/assets/577460ad-8ba3-4766-8ba5-83821edd7207)

---

#### 2.2 🚚 **Shipping Cost (H4)**
Next, i calculate the **Shipping Cost** by multiplying the **Quantity Purchased** (F4) by the shipping cost per item stored in cell **P1**. Shipping cost is constant at $5 per item, so i use an absolute reference for P1.

- **Formula**:
  ```excel
  =F4*$P$1
  ```
- **Economic Concept**:  
  **Shipping Costs** are considered **variable costs** because they fluctuate depending on how many units are sold. This impacts overall expenses, which must be deducted from total revenue to calculate profit.

- **Expected Result**: `$23,260`
![image](https://github.com/user-attachments/assets/f5ce3e29-1ecd-4190-b683-7383a6c10ca9)

---

#### 2.3 ➕ **Total Cost (I4)**
The **Total Cost** is calculated by summing the **Purchase Cost** (G4) and the **Shipping Cost** (H4).

- **Formula**:
  ```excel
  =G4+H4
  ```
- **Economic Concept**:  
  The **Total Cost** reflects both fixed and variable costs, which companies must cover to run their operations. This is essential in understanding how much a company spends on inventory and logistics.

- **Expected Result**: `$1,033,476.69`
![image](https://github.com/user-attachments/assets/7d60fd22-f93d-4279-8091-8a588cbd2d66)

---

#### 2.4 💲 **Retail Price per Item (J4)**
i calculate the **Retail Price** using a markup of 50%. This means i increase the combined cost (Wholesale + Shipping) by 1.5 to get the retail price.

- **Formula**:
  ```excel
  =(E4+$P$1)*1.5
  ```
- **Economic Concept**:  
  The **markup** is a percentage that businesses add to the cost to determine the selling price. It’s a pricing strategy used by businesses to ensure profitability.
## ℹ️ Why Multiply by 150% for a 50% Markup?
# Retail Price = Cost + (Cost × Markup Percentage)
             = Cost × (1 + 0.50)
             = Cost × 1.5
             = Cost × 150%

  - **Expected Result**: `$333.24`
---
![image](https://github.com/user-attachments/assets/5f85089d-ecf1-4c23-af71-6fc077cc01f8)

![image](https://github.com/user-attachments/assets/1f289cc2-f216-4bd6-8c79-44a230ab9eab)

---

#### 2.5 💵 **Revenue (L4)**
The **Revenue** is calculated by multiplying the **Quantity Sold** (K4) by the **Retail Price** (J4). This tells us how much money the company makes by selling the stock.

- **Formula**:
  ```excel
  =K4*J4
  ```
- **Economic Concept**:  
  **Revenue** is the total amount of money earned from sales. It is a critical metric for understanding business performance, as it is the starting point for profitability analysis.

- **Expected Result**: `$1,550,215.04`
![image](https://github.com/user-attachments/assets/d08256f2-d26e-435f-9b8c-d69ace80312a)

---

#### 2.6 💰 **Profit (M4)**
We calculate the **Profit** by subtracting the **Total Cost** (I4) from the **Revenue** (L4). This shows us how much money the company made after covering all expenses.

- **Formula**:
  ```excel
  =L4-I4
  ```
- **Economic Concept**:  
  **Profit** is the difference between total revenue and total expenses. This is the money a company keeps after covering the costs of production and sales.

- **Expected Result**: `$516,738.35`
![image](https://github.com/user-attachments/assets/f6ba8ed6-0583-4ebb-86d4-8d86d70e2b1f)

---

### 🔁 Step 3: Apply Autofill
Once i have entered the formulas for the first row, use **Autofill** to copy the formulas down to row 200. Excel will adjust the formulas based on the data in each row.

- **Tip**: If you don't see data to the left or right, manually drag the formula down.

---
![image](https://github.com/user-attachments/assets/0fc45d00-d992-4f39-90b1-ee415400dbd2)

### 📊 Step 4: Verify Results in Row 201
After applying Autofill, check that **row 201** correctly sums up all the results in columns G to M.

- **Row 201** will display the total values for **Purchase Cost**, **Shipping Cost**, **Total Cost**, **Retail Price**, **Revenue**, and **Profit**.

---

### 📈 Step 5: Calculate Gross Profit Margin (Cell P3)
To calculate the **Gross Profit Margin**, we use the formula:

- **Formula**:
  ```excel
  =(L201-I201)/L201
  ```
- **Economic Concept**:  
  The **Gross Profit Margin** tells us what percentage of revenue exceeds the cost of goods sold. It’s a key profitability metric that shows how efficient a company is in producing and selling products.

- **Expected Result**: `33.33%`
![image](https://github.com/user-attachments/assets/8c5c87fe-08a8-47bb-9f96-6640e5339de6)

---

## 🧑‍💼 Basic Economics and Math Concepts

### 📏 Basic Math Principles

1. **Order of Operations (PEMDAS)**:  
   This is the rule that tells us the order in which operations should be performed. Parentheses come first, followed by Exponents, then Multiplication/Division (left to right), and finally Addition/Subtraction (left to right).

2. **Percentage Calculations**:  
   To calculate a percentage:
   ```math
   Amount = Base * (Percentage / 100)
   ```
   This is useful for calculating markup, profit margins, and other financial ratios.

### 💡 Basic Economics Concepts

1. **Cost of Goods Sold (COGS)**:  
   This represents the direct costs involved in producing goods sold by a company. These costs include materials, labor, and shipping, and are essential for calculating profit margins.

2. **Markup**:  
   Markup refers to the percentage added to the cost of an item to determine its retail price. It's a pricing strategy used by businesses to ensure profitability.

3. **Revenue**:  
   Revenue is the total income from the sale of goods or services. It is a key indicator of business performance and is the starting point for profitability analysis.

4. **Profit**:  
   Profit is the money a company keeps after paying all its expenses. It's calculated as:
   ```math
   Profit = Revenue - Total Costs
   ```
   Understanding profit is essential to determine how well a business is doing.

5. **Gross Profit Margin**:  
   This is a profitability ratio that shows the percentage of revenue that exceeds the cost of goods sold. A higher margin indicates a more profitable business.

---

## 📚 Resources
- **Excel Workbook**: `Revenue figures.xlsx`

---


## 🧑‍💼 About Me
This README and exercise were done by me as part of my learning journey in Excel and financial modeling.  

**Author**: Henok Tariku  
📘 Student | 💻 Microsoft Power BI -Excel Learner 


## 🧑‍💼 About Me
This README and exercise were done by me as part of my learning journey in Excel and financial modeling.  

**Author**: Henok Tariku  
📘 Student | 💻 Excel Learner | 📊 Financial Modeling Explorer


