
# 📊 Excel Exercise: Standardizing Text-Based Data

## 📝 Overview

This project demonstrates how to clean and standardize text-based data using **text functions** in Microsoft Excel. The source file, `Reseller Information.xlsx`, contains inconsistent text entries such as extra spaces, improper casing, and concatenated data. The goal was to use Excel formulas to:

- Remove unnecessary spaces
- Correct text casing
- Extract specific substrings
- Combine text with formatting
- Replace formulas with static values
- Delete obsolete data columns



## 📁 Step 1: Download the File

Open the file: `Reseller Information.xlsx`.  
Go to the sheet named **Reseller Details**, which contains pre-filled data without formulas.



## 🛠 Step 2: Create the Calculations

### ✅ TRIM Function (Remove Spaces)

In cell `C2`, remove leading/trailing spaces from `B2`:

```excel
=TRIM(B2)
```

🔹 **Output:** `The Bicycle Accessories Company`
![image](https://github.com/user-attachments/assets/29640379-08e1-4b28-96b9-f15f6f879da0)




### ✅ PROPER Function (Correct Casing)

In cell `E2`, fix all-uppercase city names in `D2`:

```excel
=PROPER(D2)
```

🔹 **Output:** `Alhambra`

![image](https://github.com/user-attachments/assets/cf2efe2a-1663-4d5d-bf9f-ce7e86b38182)


### ✅ LEFT Function (Extract Start)

In `I2`, extract `"States"` from the start of text in `H2`:

```excel
=LEFT(H2,6)
```

🔹 **Output:** `States`

![image](https://github.com/user-attachments/assets/a422cf53-4076-49b0-a052-04f5c9970225)


### ✅ RIGHT Function (Extract End)

In `J2`, extract `"New York"` from the end of text in `H2`:

```excel
=RIGHT(H2,8)
```

🔹 **Output:** `New York`

![image](https://github.com/user-attachments/assets/e518188a-6347-444c-9140-980dff7d1c2a)


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

![image](https://github.com/user-attachments/assets/758c2fc4-2ac9-4024-84cc-0b7c91f85b59)


### ✅ MID Function (Extract Middle)

In `L2`, extract `"uSA"` from `H2` starting at character 8:

```excel
=MID(H2, 8, 3)
```

🔹 **Output:** `uSA`

![image](https://github.com/user-attachments/assets/661cca6d-4949-4026-8be3-74934fd5b611)


### ✅ UPPER Function (Make Uppercase)

In `M2`, convert `uSA` (in `L2`) to uppercase:

```excel
=UPPER(L2)
```

🔹 **Output:** `USA`
![image](https://github.com/user-attachments/assets/eca10aa3-d2e5-4bf5-ae59-521e7e26a900)




## 🔁 Step 3: Autofill All Formulas

Use the **Autofill double-click** method to copy formulas in `C2`, `E2`, `I2`, `J2`, `K2`, `L2`, and `M2` down to row 428.



## 📋 Step 4: Paste Formulas as Values

1. Highlight columns `C`, `E`, `I`, `J`, `K`, `L`, and `M`
2. Press `Ctrl + C` to copy
3. Go to **Home > Paste > Paste Values**

This step removes formulas and keeps only results.



## 🧹 Step 5: Clean Up

Delete the following columns:

- `B` – Original company names
- `D` – Original city names
- `G` – Part 1 of combined country
- `H` – Concatenated string
- `I`, `L` – Intermediate extracted columns



## ✅ Final Result

My final sheet will contain:

- Cleaned company names
- Properly capitalized cities
- Extracted and formatted country and state data
- Only static values (no formulas)
- All redundant data removed

![image](https://github.com/user-attachments/assets/d087c52a-af02-4c43-a527-fbe43ef8de92)





## 🎉 Conclusion

I successfully applied the following Excel text functions:

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


