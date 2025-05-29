
# Final Course Project: Creating an Executive Data Summary

## 📌 Introduction

Over the past three weeks, I learned how to work with Microsoft Excel—formatting data, using functions, and performing calculations. In this final project, I applied those skills to help Jamie from Adventure Works prepare an executive summary of sales data for Q1.



## 🧾 Case Study: Adventure Works Sales Report

Jamie was preparing for a management meeting and needed an Excel worksheet that shows sales for Q1 (Quarter One) in both 2022 and 2023. My task was to:

- Calculate total Q1 sales for both years.
- Calculate the percentage increase in 2023.
- Break down these totals by month.
- Organize and format the data for executive presentation.



## ✅ Step-by-Step Instructions

### 🔹 Step 1: Download and Review the File

- I downloaded the `Quarter One Report.xlsx` file.
- I opened the worksheet named `Summary`.



### 🔹 Step 2: Add and Format Headings

1. I widened column **A** to fit the contents of cells **A12 to A14**.
2. I added a new blank column before **column E**.
3. In **cell A4**, I typed `TOTAL Q1 SALES`.
4. In **cell A10**, I typed `Q1 MONTHLY TOTALS`.
5. I formatted `A4`:
   - Increased font size by one level
   - Made it bold
   - Added a background color
   - Merged & Centered across `A4:D4`
6. I used **Format Painter** to apply the same format to **A10**.
   ![image](https://github.com/user-attachments/assets/d4d0be28-8adc-47f0-aba5-05a5913a770c)

8. I bolded and wrapped text for headings in:
   - `B5`, `C5`, `D5`
   - `B11`, `C11`, `D11` (using Format Painter)
   ![image](https://github.com/user-attachments/assets/b611d22f-9f2f-4092-a510-b5ed3b604b20)

### Note on Merged & Centered Across Selection

The Excel feature **"Merge & Center Across Selection"** does not work directly from the ribbon button.

Instead, I used this method:

- Select the cells `A4:D4`
- Right-click → Format Cells → Alignment tab
- Under Horizontal, choose **Center Across Selection**
- Click OK

This centers the text across the cells without merging them.

For the border, I set the border style to **None** to keep the area clean.

  ![image](https://github.com/user-attachments/assets/d6f06577-9cdb-44a6-b2b6-9a65eab7ba0d)


### 🔹 Step 3: Clean and Reorganize Data

1. In **cell H2**, I used the `PROPER` function:

```excel
=PROPER(G2)
```

2. I autofilled down the column, copied the entire column, and used Paste Values.
   ![image](https://github.com/user-attachments/assets/d143625f-314c-4c78-8a72-49eb9e692ac8)

4. I deleted column G.
   ![image](https://github.com/user-attachments/assets/c0dd13dc-7f63-4bad-8b64-1af52cd36150)

   
6. I selected the range F2:Y246 and sorted it by Order Date (Oldest to Newest) using the Sort dialog.
# 📊 Sorting the Sales Data in Excel

## ✅ Goal
Sort the sales records by **Order Date** from **oldest to newest** so that the monthly total calculations in later steps work correctly.

---

## 🤔 My Confusion

At first, I was confused because I thought I could just click the **A→Z sort button** on the **Data ribbon**. But when I did that, **only part of the data was sorted**. The rest of the rows didn’t move properly.

Later, I realized the problem was caused by a **blank column (column E)** that broke the full range of data. Excel treats blank columns as a "stop" point when using the quick sort buttons.

---

## ⚠️ Important Note

> **Don’t use the A→Z or Z→A sort buttons directly** if there are blank columns. Excel won’t select the full dataset correctly.

---

## ✅ What I Did Instead

To fix it and sort everything correctly:

1. **Click on cell F2** (first data cell after the blank column).
2. Press `Ctrl + Shift + End` to select the entire block of data (F2 to the last cell).
3. Go to the **Data** tab.
4. Click the full **Sort** button (NOT A→Z).
5. In the Sort window:
   - Make sure “**My data has headers**” is checked ✅
   - Under **Sort By**, choose `Order Date`
   - Under **Order**, select `Oldest to Newest`
6. Click **OK**.

---

## ✅ Final Result

All rows are now sorted by date correctly, and the summary section on the left side (columns A–D) remains untouched.

---

## 💡 Tip
When working with data that has blank columns, **always highlight the full block manually** before sorting.
Use the shortcut `Ctrl + Shift + End` to speed up the selection.

![image](https://github.com/user-attachments/assets/42db022b-607a-43fe-94f0-fc018ea0aba5)
![Uploading image.png…]()


7. I hid:
   - Column F
   - Columns S to Y
8. I froze panes from cell G2.



### 🔹 Step 4: Create New Row Information

- I extracted the Month in cell K2:

```excel
=MONTH(J2)
```

- I extracted the Year in cell L2:

```excel
=YEAR(J2)
```

- I autofilled both down to row 246.

- In cell P2, I calculated the total order value:

```excel
=M2 * N2
```

- In cell Q2, I applied a tax rule using `IF`:

```excel
=IF(P2 > 2000, P2 * 0.05, 0)
```

---

### 🔹 Step 5: Calculate and Compare Profit Margins

#### Total Q1 Sales by Year

- In B6:

```excel
=SUMIFS(R2:R246, L2:L246, 2022)
```

- In C6:

```excel
=SUMIFS(R2:R246, L2:L246, 2023)
```

#### Monthly Breakdown (Q1)

- In B12 (January 2022):

```excel
=SUMIFS($R$2:$R$103, $K$2:$K$103, 1)
```

- In B13 (February 2022):

```excel
=SUMIFS($R$2:$R$103, $K$2:$K$103, 2)
```

- In B14 (March 2022):

```excel
=SUMIFS($R$2:$R$103, $K$2:$K$103, 3)
```

- In C12 (January 2023):

```excel
=SUMIFS($R$104:$R$246, $K$104:$K$246, 1)
```

- In C13 (February 2023):

```excel
=SUMIFS($R$104:$R$246, $K$104:$K$246, 2)
```

- In C14 (March 2023):

```excel
=SUMIFS($R$104:$R$246, $K$104:$K$246, 3)
```

#### Percentage Change in Sales

- In D6 (Yearly change):

```excel
=(C6 - B6) / B6
```

- In D12 to D14 (Monthly change):

```excel
=(C12 - B12) / B12
```

---

## 🏁 Conclusion

I successfully formatted and cleaned data, calculated key figures using formulas, and created an executive summary that visually and analytically compares Q1 sales for 2022 and 2023. These insights are now ready for presentation at the management meeting.

