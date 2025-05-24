
# 📊 Advertising Campaign USA Dates - Excel Automation

## 📁 Project Overview

This project helps track and calculate key milestone dates for five USA-based advertising campaigns using Microsoft Excel functions. You will use date and time functions to calculate:

- 📅 Number of **calendar days** until the campaign deadline
- 🗓️ Number of **working days** (excluding weekends and U.S. holidays)
- 📆 The **month** and **year** of the campaign deadline



## 📂 File Used

**File Name:** `Advertising Campaign USA Dates.xlsx`  
**Sheet Name:** `USA Launch Dates`  
**Columns Included:**
- Column B: Today's Date (Cell B1)
- Column C: Start Date
- Column D: Deadline Date
- Column J5:J26: U.S. Federal Holidays (2023–2024)

> ⚠️ **Important:** The spreadsheet uses U.S. date format: `MM/DD/YYYY`.  
> If your system uses `DD/MM/YYYY`, manually retype the dates to avoid calculation errors.

---

## 🛠️ Step-by-Step Instructions

### ✅ Step 1: Set Today’s Date

In **cell B1**, enter today’s date as a **static value** instead of a formula:

```text
05/09/23
```

This is used for consistency with the example results.

![image](https://github.com/user-attachments/assets/65ac5823-a286-45c9-aee9-819ceffecddd)


### ➗ Step 2: Calculate Calendar Days Until Deadline

In **cell E5**, calculate the number of **calendar days** between today's date and the deadline:

```excel
=D5 - $B$1
```

- `$B$1`: Absolute reference to ensure it stays fixed when copying the formula down.
- `D5`: Deadline date for the current row.

![image](https://github.com/user-attachments/assets/cf4b4b56-4f76-4ef4-b80c-88032723104d)

![image](https://github.com/user-attachments/assets/953c8857-4e7d-4ebc-b813-649e3a7a23cd)

### 📅 Step 3: Calculate Working Days Until Deadline

In **cell F5**, use the `NETWORKDAYS` function to exclude weekends and holidays:

```excel
=NETWORKDAYS($B$1, D5, $J$5:$J$26)
```

- `$B$1`: Today's date
- `D5`: Deadline date
- `$J$5:$J$26`: Federal holidays (fixed range)

This returns the number of business days between today and the deadline.

![image](https://github.com/user-attachments/assets/619b35fd-8c1e-42d8-a793-e16fee4c4beb)



### 🗓️ Step 4: Extract Launch Month

In **cell G5**, extract the **month** of the deadline using the `MONTH` function:

```excel
=MONTH(D5)
```

![image](https://github.com/user-attachments/assets/61ca7b01-90ce-4d86-81c5-0c5925ef5ef0)


### 📆 Step 5: Extract Launch Year

In **cell H5**, extract the **year** of the deadline using the `YEAR` function:

```excel
=YEAR(D5)
```

![image](https://github.com/user-attachments/assets/c4b16fb4-f265-4317-894d-6ae2868e521b)


### 🔁 Step 6: Copy Formulas Down

Apply your formulas from row 5 to rows 6 through 9:

1. Select cells **E5:H5**
2. Hover over the bottom-right corner until you see the **fill handle** (black cross)
3. **Double-click** the fill handle to autofill down to row 9

---

## ✅ Final Result

Once completed, your spreadsheet will automatically show:

| Campaign | Start Date | Deadline | 📅 Days to Deadline | 🗓️ Working Days | 📆 Month | 📆 Year |
|----------|------------|----------|---------------------|-----------------|----------|---------|
| ...      | ...        | ...      | (E column result)   | (F column)      | (G)      | (H)     |

Lucas can now easily plan and coordinate the campaign launch schedule with accurate timelines.

![image](https://github.com/user-attachments/assets/04a9ed04-30a4-49f5-b66c-be800fc1ea10)

## 📘 Excel Functions Used

| Function        | Description                                                |
|----------------|------------------------------------------------------------|
| `TODAY()`       | Returns the current date (used initially)                 |
| `NETWORKDAYS()` | Calculates working days excluding weekends and holidays   |
| `MONTH()`       | Extracts the numeric month from a date                    |
| `YEAR()`        | Extracts the year from a date                             |


## 💾 Notes

- Use **absolute references** (with `$`) for static cells (e.g., `$B$1`, `$J$5:$J$26`) to ensure formulas copy correctly.
- Double-check system regional settings if date formats appear inconsistent.
- we can reuse this method for other regional campaigns by adjusting the start and deadline dates.
