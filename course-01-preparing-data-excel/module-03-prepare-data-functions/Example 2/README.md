# 📅 Excel Date and Time Functions for Windows Users

## 🧭 Introduction

Working with **date and time** in Excel is a common yet powerful skill. This guide covers essential functions to help you perform **date-based calculations**, **time tracking**, **project planning**, and more. Dates and times in Excel are stored as numbers, making them ideal for calculations and automation in your spreadsheets.



## ⏱️ How Date and Time Are Tracked in Excel

- Excel stores **dates** as serial numbers starting from **January 1, 1900**.
  - For example, `01/01/1900` is `1`, `01/02/1900` is `2`, and so on.
- **Time** is stored as a fraction of a day.
  - Example: `0.5` equals 12:00 noon.

To enter a date:

```plaintext
MM/DD/YY → Example: 08/30/23
```

To enter time:

```plaintext
HH:MM → Example: 10:30
```

📝 Note: Date and time values entered directly are static. Use dynamic functions for real-time updates.



## 📆 Dynamic Date and Time Functions

### ✅ TODAY()

Displays the current system date and updates daily.

```excel
=TODAY()
```
![image](https://github.com/user-attachments/assets/956e6486-1b46-4c81-a81c-ff2bf689f317)

### ✅ NOW()

Displays the current system **date and time** and updates when recalculated.

```excel
=NOW()
```

> 🪟 **Windows Tip**: Press `F9` to refresh NOW().


![image](https://github.com/user-attachments/assets/a82a54fc-60ab-4b53-bf71-745b37bfafaa)

## 🧩 Extracting Date Components

You can break down a full date into day, month, or year using these functions:

### DAY

```excel
=DAY(A2)
```

Returns the day from the date in cell `A2`.
![image](https://github.com/user-attachments/assets/b08cf2b0-5055-4e2a-a9cf-b235f565db1e)


### MONTH

```excel
=MONTH(A2)
```

Returns the month from the date in cell `A2`.

![image](https://github.com/user-attachments/assets/aa4be43d-6bf0-44f3-9c37-faf82f0f38b9)

### YEAR

```excel
=YEAR(A2)
```

Returns the year from the date in cell `A2`.

![image](https://github.com/user-attachments/assets/19610e76-4a1e-45ca-99a5-8800de89616b)



## 📅 NETWORKDAYS – Calculate Working Days

Used to count workdays between two dates, excluding weekends.

```excel
=NETWORKDAYS(A2, B2)
```

- `A2`: Start date  
- `B2`: End date
![image](https://github.com/user-attachments/assets/c8387985-cfe3-442b-a4c2-31ceb78b96a8)


### 📆 Including Holidays

```excel
=NETWORKDAYS(A2, B2, H2:H12)
```

- `H2:H12`: List of holiday dates to exclude.

![image](https://github.com/user-attachments/assets/13b316a0-7089-46d0-bcbb-5070ccfaa72a)


## 🧱 DATE – Combine Year, Month, Day

Used to build a valid date from individual cells.

```excel
=DATE(C2, A2, B2)
```

- `C2`: Year  
- `A2`: Month  
- `B2`: Day

## 🛠️ Fixing the Excel DATE Function

If your **Year**, **Month**, and **Day** are in separate cells:

- `A2` = Month (e.g., 5)
- `B2` = Day (e.g., 24)
- `C2` = Year (e.g., 2025)

✅ Use this correct formula:
```excel
=DATE(C2, A2, B2)
```

⛔ Incorrect (causes wrong date):
```excel
=DATE(C2, B2, C2)
```

📅 Correct Output: `5/24/2025` (May 24, 2025)

![image](https://github.com/user-attachments/assets/64a086f0-3167-40c5-b63e-5c3e2c765289)


## 📊 DATEDIF – Difference Between Dates

A legacy function to calculate the difference in days, months, or years.

### Difference in Years

```excel
=DATEDIF(B2, C2, "y")
```

- `B2`: Start date  
- `C2`: End date (can be `=TODAY()` for dynamic updates)  
- `"y"`: Unit of time to calculate (`"y"` = years, `"m"` = months, `"d"` = days)

📌 **Important**: You must **type DATEDIF manually**; it's not in the function wizard.

![image](https://github.com/user-attachments/assets/340d0528-887f-42be-8772-da28478569b5)


## ✅ Summary of Functions

| Function               | Purpose                          | Syntax Example                          |
|------------------------|----------------------------------|------------------------------------------|
| `TODAY()`              | Current system date              | `=TODAY()`                               |
| `NOW()`                | Current date & time              | `=NOW()`                                 |
| `DAY()`                | Extract day                      | `=DAY(A2)`                               |
| `MONTH()`              | Extract month                    | `=MONTH(A2)`                             |
| `YEAR()`               | Extract year                     | `=YEAR(A2)`                              |
| `NETWORKDAYS()`        | Count working days               | `=NETWORKDAYS(A2, B2)`                   | |
| `DATE()`               | Combine year, month, day         | `=DATE(C2, A2, B2)`                      |
| `DATEDIF()`            | Date difference (legacy)         | `=DATEDIF(B2, C2, "y")`                  |

---

## 🔚 Conclusion

Excel provides a robust set of tools for working with date and time data. By mastering these functions, you can automate time tracking, plan schedules, and generate real-time reports with ease. Whether you're managing projects or organizing data by timeline, these formulas will elevate your spreadsheet capabilities.
