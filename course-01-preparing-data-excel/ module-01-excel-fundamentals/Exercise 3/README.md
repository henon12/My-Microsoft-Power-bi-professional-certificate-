# 📊 Filtering Data in Microsoft Excel — Adventure Works Inventory

## 📝 Overview

This exercise demonstrates how to filter data in Microsoft Excel using the **Adventure Works Inventory1.xlsx** file. The goal is to answer specific questions using Excel's filter features.

> 🕒 **Note:** This task was originally set for data in the year **2023**, but since this file was opened in **2025**, date-based results may vary due to dynamic filtering based on system dates.

---

## 🔧 Step-by-Step Instructions

### Step 1: Getting Started
- Open the `Adventure Works Inventory1.xlsx` file in Microsoft Excel.
- Make sure you are on the **Products** worksheet.

📷 **Screenshot:** Workbook opened  
![Step 1 - Open Excel File](https://github.com/user-attachments/assets/c59e8e59-e895-448e-96cf-7b5fb7903fcc)

---

### Step 2: Enable Filtering
- Go to the **Data** tab and click the **Filter** button to activate dropdowns on each column heading.

📷 **Screenshot:** Filter feature activated  
![Step 2 - Enable Filter](https://github.com/user-attachments/assets/efe9a87b-e0f2-432e-bcfb-4bf7738227ba)

---

## 🔍 Data Extraction Tasks

### ✅ 1. Listings for Gear Components
- Click the filter arrow in the **Category** column.
- Deselect all and check only **Gear Components**.

📷 **Screenshot:** Filter by Gear Components  
![Step 3 - Filter Gear Components](https://github.com/user-attachments/assets/4e3fdda2-049e-4e4d-a510-3df5e815f589)

📷 **Screenshot:** Result — 20 rows displayed  
![Step 3 - Result](https://github.com/user-attachments/assets/5e0e6841-44ac-4f4a-b728-4d64a77c8eb8)

---

### ✅ 2. Orders Placed with Z123 in 2025
- Filter **Supplier** column for **Z123**.
- Filter **Date Entered** column for the year **2025**.

📷 **Screenshot:** Filter by Supplier Z123  
![Step 4 - Filter Z123](https://github.com/user-attachments/assets/5898ba7d-07a3-48b1-bf73-ad5b97262cda)

📷 **Screenshot:** Filter by Date Entered (2025)  
![Step 4 - Filter by 2025](https://github.com/user-attachments/assets/aafbafb3-c5a9-42c9-86a5-d0da319d114c)

📷 **Screenshot:** Result — 6 records  
![Step 4 - Result](https://github.com/user-attachments/assets/df98c58f-d564-4dbd-b145-c7a71baf77f7)

---

### ✅ 3. Orders Placed with Z123 in 2022
- Keep **Supplier** as Z123.
- Change **Date Entered** filter to only include **2022**.

📷 **Screenshot:** Filter by 2022  
![Step 5 - Filter by 2022](https://github.com/user-attachments/assets/d0dd3c7d-1934-4932-a8ef-4587dea6dda5)

📷 **Screenshot:** Result — 2 records  
![Step 5 - Result](https://github.com/user-attachments/assets/4dae26fc-73c1-4b0e-9ae3-245c5b105397)

---

### ✅ 4. Orders for Mountain Bike Frames
- Use **Text Filters > Contains** in the **Product Name** column.
- Enter keyword: `mountain`.

📷 **Screenshot:** Text Filter on Product Name  
![Step 6 - Text Filter Mountain](https://github.com/user-attachments/assets/3c65dbed-b999-4eb6-93e3-3db1b6ed95b6)

📷 **Screenshot:** Result — 22 rows  
![Step 6 - Result](https://github.com/user-attachments/assets/7c79d518-d885-4f03-9436-d00e1e23c02d)

---

### ✅ 5. Mountain Bike Orders with Stock Over 500
- Keep the "mountain" text filter.
- Use **Number Filter > Greater Than** on **Units in Stock** and enter `500`.

📷 **Screenshot:** Number Filter on Stock  
![Step 7 - Number Filter Stock](https://github.com/user-attachments/assets/ea31ac4a-4e82-4b26-9bb0-cbff4a3b43da)

📷 **Screenshot:** Result — 3 rows  
![Step 7 - Result](https://github.com/user-attachments/assets/fbd6cefc-d172-4e0f-bd55-15a2481d6f0a)

---

## 🎬 Additional Resources

- 📹 [Sorting and Filtering Data in Excel – Microsoft Support](https://support.microsoft.com/excel)

---

## 📁 File Used

- `Adventure Works Inventory1.xlsx`

---

## 🧠 Conclusion

By completing this exercise, you’ve practiced essential Excel filtering techniques:
- Basic column filters
- Text and number filtering
- Multi-level filter logic

These are foundational for data analysis and useful in a wide variety of business and technical workflows.

---

## 📸 Screenshot Folder

If working offline, keep screenshots in a `screenshots/` folder and name them consistently (e.g., `step1-open-excel.png`, etc.).
