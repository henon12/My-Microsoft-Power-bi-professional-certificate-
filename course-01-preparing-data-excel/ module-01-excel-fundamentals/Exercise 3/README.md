# 📊 Filtering Data in Microsoft Excel — Adventure Works Inventory

## 📝 Overview

This exercise demonstrates how to filter data in Microsoft Excel using the **Adventure Works Inventory1.xlsx** file. The goal is to answer specific questions using Excel's filter features.

> 🕒 **Note:** This task was originally set for data in the year **2023**, but since this file was opened in **2025**, date-based results may vary due to dynamic filtering based on system dates.



## 🔧 Step-by-Step Instructions

### Step 1: Getting Started
- Open the `Adventure Works Inventory1.xlsx` file in Microsoft Excel.
- Make sure you are on the **Products** worksheet.

📷 **Screenshot:** Workbook opened  
![Step 1 - Open Excel File](https://github.com/user-attachments/assets/c59e8e59-e895-448e-96cf-7b5fb7903fcc)



### Step 2: Enable Filtering
- Go to the **Data** tab and click the **Filter** button to activate dropdowns on each column heading.

📷 **Screenshot:** Filter feature activated  
![Step 2 - Enable Filter](https://github.com/user-attachments/assets/efe9a87b-e0f2-432e-bcfb-4bf7738227ba)


## 🔍 Data Extraction Tasks

### ✅ 1. Listings for Gear Components
- Click the filter arrow in the **Category** column.
- Deselect all and check only **Gear Components**.

📷 **Screenshot:** Filter by Gear Components  
![Step 3 - Filter Gear Components](https://github.com/user-attachments/assets/4e3fdda2-049e-4e4d-a510-3df5e815f589)

📷 **Screenshot:** Result — 20 rows displayed  
![Step 3 - Result](https://github.com/user-attachments/assets/5e0e6841-44ac-4f4a-b728-4d64a77c8eb8)



### ✅ 2. Orders Placed with Z123 in 2025
- Filter **Supplier** column for **Z123**.
- Filter **Date Entered** column for the year **2025**.

📷 **Screenshot:** Filter by Supplier Z123  
![Step 4 - Filter Z123](https://github.com/user-attachments/assets/5898ba7d-07a3-48b1-bf73-ad5b97262cda)

📷 **Screenshot:** Filter by Date Entered (2025)  
![Step 4 - Filter by 2025](https://github.com/user-attachments/assets/aafbafb3-c5a9-42c9-86a5-d0da319d114c)

📷 **Screenshot:** Result — 6 records  
![Step 4 - Result](https://github.com/user-attachments/assets/df98c58f-d564-4dbd-b145-c7a71baf77f7)



### ✅ 3. Orders Placed with Z123 in 2022
- Keep **Supplier** as Z123.
- Change **Date Entered** filter to only include **2022**.

📷 **Screenshot:** Filter by 2022  
![Step 5 - Filter by 2022](https://github.com/user-attachments/assets/d0dd3c7d-1934-4932-a8ef-4587dea6dda5)

📷 **Screenshot:** Result — 2 records  
![Step 5 - Result](https://github.com/user-attachments/assets/4dae26fc-73c1-4b0e-9ae3-245c5b105397)



### ✅ 4. Orders for Mountain Bike Frames
- Use **Text Filters > Contains** in the **Product Name** column.
- Enter keyword: `mountain`.

📷 **Screenshot:** Text Filter on Product Name  
![Step 6 - Text Filter Mountain]![image](https://github.com/user-attachments/assets/b9a59d03-a223-46d4-85e3-7194a6c74e35)

![image](https://github.com/user-attachments/assets/dcae4849-eb84-40e9-966b-318cf7633731)
📷 **Screenshot:** Result — 22 rows  
![Step 6 - Result](https://github.com/user-attachments/assets/0c985fbf-b087-4886-8965-f21db384999d)




### ✅ 5. Mountain Bike Orders with Stock Over 500
- Keep the "mountain" text filter.
- Use **Number Filter > Greater Than** on **Units in Stock** and enter `500`.

📷 **Screenshot:** Number Filter on Stock  
![Step 7 - Number Filter Stock](https://github.com/user-attachments/assets/459ec93e-3f18-4911-9684-3d90a99c817b)

![image](https://github.com/user-attachments/assets/babda52a-acbd-4991-bcb9-4fcd66ea45c3)

📷 **Screenshot:** Result — 3 rows  

![Step 7 - Result](https://github.com/user-attachments/assets/83aebd99-e12c-4a78-9a58-46a54c32e5b5)





## 🎬 Additional Resources

- 📹 [Sorting and Filtering Data in Excel – Microsoft Support][(https://support.microsoft.com/excel](https://support.microsoft.com/en-gb/office/sort-data-in-a-range-or-table-62d0b95d-2a90-4610-a6ae-2e545c4a4654))



## 📁 File Used

- `Adventure Works Inventory1.xlsx`



## 🧠 Conclusion

By completing this exercise, you’ve practiced essential Excel filtering techniques:
- Basic column filters
- Text and number filtering
- Multi-level filter logic

These are foundational for data analysis and useful in a wide variety of business and technical workflows.



