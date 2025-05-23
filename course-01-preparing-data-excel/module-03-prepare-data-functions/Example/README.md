
# Excel Text Standardization Functions

This guide provides a comprehensive overview of functions that can be used to clean and standardize text data in Microsoft Excel. These functions help ensure consistency and improve data quality for analysis.


## 📌 Introduction

Working with unstructured text data often leads to errors and inconsistencies. Excel provides powerful built-in functions to clean and format text for better accuracy in reports, summaries, and databases.


## 🎯 Learning Objectives

- Understand Excel functions available for adjusting and cleaning text data
- Learn to write correct and reliable formulas
- Apply functions to solve real-world formatting issues


## 🧑‍💼 Scenario: Jamie at Adventure Works

Jamie works at Adventure Works and manages customer records. Their data contains unnecessary characters, inconsistent formats, and merged text fields. Jamie uses Excel functions to clean and standardize the text data effectively.



## 🔧 Key Excel Text Functions

### 1. `LEFT`, `RIGHT`, and `MID` Functions

Extract specific parts of a string based on character positions.

| Function | Description |
|----------|-------------|
| `LEFT(text, num_chars)` | Extracts characters from the start |
| `RIGHT(text, num_chars)` | Extracts characters from the end |
| `MID(text, start_num, num_chars)` | Extracts characters from the middle |

**Example:**  
If B2 contains `"Doctor Martin Garcia"`  
- `=LEFT(B2;6)` → `Doctor`  
- `=MID(B2;8;6)` → `Martin`  
- `=RIGHT(B2;6)` → `Garcia`

🔹 *Tip:* You can also use Excel's **Text to Columns** tool to split text quickly.

![image](https://github.com/user-attachments/assets/6787f86d-916e-4e96-8226-d746be148cb2)
![image](https://github.com/user-attachments/assets/f2d7858a-ab23-4929-ba82-fd8a9fdf0035)
![image](https://github.com/user-attachments/assets/b0d8dc48-210c-4dd1-a8ff-544b228f96df)




### 2. `TRIM` Function

Removes extra spaces from text (leading, trailing, or multiple in-between).

**Syntax:**  
```excel
=TRIM(B2)
```

**Steps to Clean a Column:**
1. Insert a new column.
2. Apply `=TRIM(A2)` and autofill.
3. Copy the results and paste as values.

![image](https://github.com/user-attachments/assets/4d0242fe-057f-418a-8a93-f36d026f20da)


![image](https://github.com/user-attachments/assets/373c08ea-8c1e-4063-9bb2-5c2477efcb82)


### 3. `UPPER`, `LOWER`, and `PROPER` Functions

Standardize the casing of text for consistency.

| Function | Output |
|----------|--------|
| `=UPPER(B2)` | ALL CAPS |
![image](https://github.com/user-attachments/assets/c6fa9f74-af29-48a7-9440-5497f17ee002)

| `=LOWER(B2)` | all lowercase |
![image](https://github.com/user-attachments/assets/52be95a1-aaac-4335-ae22-1d03848d4bbb)

| `=PROPER(B2)` | Capitalizes Each Word |
![image](https://github.com/user-attachments/assets/ed6ccefd-bdcd-4db4-9a43-ab1f7040b94a)




### 4. `CONCAT` Function

Joins values from multiple cells into one.

**Syntax:**
```excel
=CONCAT(A2, " ", B2, " ", C2)
```

- Joins “Doctor”, “Martin”, “Garcia” → `Doctor Martin Garcia`
- Older version: `CONCATENATE(A2, " ", B2, " ", C2)`

![image](https://github.com/user-attachments/assets/91710718-9206-4647-966f-1d30d22ec1a9)
![image](https://github.com/user-attachments/assets/38ca8256-31da-4d08-b7bd-ee90f7259773)



## 🌍 Regional Settings in Excel

- Excel function syntax may differ by **region or language**.
- Common differences:
  - **USA:** Date format = `MM/DD/YYYY`, separator = `,`
  - **Europe:** Date format = `DD/MM/YYYY`, separator = `;`

**How to Adjust:**
- **Excel Settings:** File → Options → Advanced
- **System Settings (Windows/Mac):** Change regional format



## ✅ Conclusion

By using Excel text functions like `TRIM`, `LEFT`, `RIGHT`, `MID`, `UPPER`, `LOWER`, `PROPER`, and `CONCAT`, you can:

- Clean text fields
- Standardize data formats
- Split or merge values
- Improve data quality for better decision-making



## 🧠 Pro Tip

Use these functions in combination to build powerful formulas and automate text cleaning tasks.



## 📚 References

- Microsoft Excel Documentation: https://support.microsoft.com/excel
- ExcelJet Function Guide: https://exceljet.net

