
# 📊 Excel Exercise: Standardizing Text-Based Data

## 📝 Overview

This project demonstrates how to clean and standardize text-based data using **text functions** in Microsoft Excel. The source file, `Reseller Information.xlsx`, contains inconsistent text entries such as extra spaces, improper casing, and concatenated data. The goal was to use Excel formulas to:

- Remove unnecessary spaces
- Correct text casing
- Extract specific substrings
- Combine text with formatting
- Replace formulas with static values
- Delete obsolete data columns

---

## 📁 Step 1: Download the File

Open the file: `Reseller Information.xlsx`.  
Go to the sheet named **Reseller Details**, which contains pre-filled data without formulas.

---

## 🛠 Step 2: Create the Calculations

### ✅ TRIM Function (Remove Spaces)

In cell `C2`, remove leading/trailing spaces from `B2`:

```excel
=TRIM(B2)
```

🔹 **Output:** `The Bicycle Accessories Company`

---

### ✅ PROPER Function (Correct Casing)

In cell `E2`, fix all-uppercase city names in `D2`:

```excel
=PROPER(D2)
```

🔹 **Output:** `Alhambra`

---

### ✅ LEFT Function (Extract Start)

In `I2`, extract `"States"` from the start of text in `H2`:

```excel
=LEFT(H2,6)
```

🔹 **Output:** `States`

---

### ✅ RIGHT Function (Extract End)

In `J2`, extract `"New York"` from the end of text in `H2`:

```excel
=RIGHT(H2,8)
```

🔹 **Output:** `New York`

---

### ✅ CONCAT Function (Combine With Space)

In `K2`, combine `G2` (`United`) and `I2` (`States`) with a space:

❌ Incorrect:

```excel
=CONCAT(G2,I2)
```

✅ Correct:

```excel
=CONCAT(G2, " ", I2)
```

🔹 **Output:** `United States`

---

### ✅ MID Function (Extract Middle)

In `L2`, extract `"uSA"` from `H2` starting at character 8:

```excel
=MID(H2, 8, 3)
```

🔹 **Output:** `uSA`

---

### ✅ UPPER Function (Make Uppercase)

In `M2`, convert `uSA` (in `L2`) to uppercase:

```excel
=UPPER(L2)
```

🔹 **Output:** `USA`

---

## 🔁 Step 3: Autofill All Formulas

Use the **Autofill double-click** method to copy formulas in `C2`, `E2`, `I2`, `J2`, `K2`, `L2`, and `M2` down to row 428.

---

## 📋 Step 4: Paste Formulas as Values

1. Highlight columns `C`, `E`, `I`, `J`, `K`, `L`, and `M`
2. Press `Ctrl + C` to copy
3. Go to **Home > Paste > Paste Values**

This step removes formulas and keeps only results.

---

## 🧹 Step 5: Clean Up

Delete the following columns:

- `B` – Original company names
- `D` – Original city names
- `G` – Part 1 of combined country
- `H` – Concatenated string
- `I`, `L` – Intermediate extracted columns

---

## ✅ Final Result

Your final sheet will contain:

- Cleaned company names
- Properly capitalized cities
- Extracted and formatted country and state data
- Only static values (no formulas)
- All redundant data removed

---

## 🎉 Conclusion

You successfully applied the following Excel text functions:

| Function | Purpose |
|----------|---------|
| `TRIM()` | Removes leading/trailing spaces |
| `PROPER()` | Capitalizes first letter of each word |
| `LEFT()` | Extracts characters from the start |
| `RIGHT()` | Extracts characters from the end |
| `MID()` | Extracts characters from the middle |
| `UPPER()` | Converts to uppercase |
| `CONCAT()` | Combines text entries |

This process is critical when working with messy real-world datasets to ensure consistency and reliability in reports and analyses.

---

**✔ Tip:** You can revisit the reading **Functions that can be used to standardize text data** for a refresher on how each function works.

---
