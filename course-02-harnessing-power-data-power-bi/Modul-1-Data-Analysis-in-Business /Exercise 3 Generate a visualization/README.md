# ✅ Exercise: Generate a Visualization – My Answer
![image](https://github.com/user-attachments/assets/1973a65a-4160-432f-a013-f2c2955a0c49)


## 🔷 Case Study (in my own words)
My manager at Adventure Works, Adio, gave me a large dataset with information about sales, order statuses, and product performance for the past month. Since the data is huge, it’s hard to understand just by looking at rows and columns. So, I used Microsoft Power BI to create visualizations. This helped me and my team clearly see how the company is performing and where we can improve. It also made it easier to make decisions using data.



## 🔷 Step 1: Import Data

**What I did:**
- I opened **Microsoft Power BI Desktop**.
- Then I selected **Home > Get Data > Text/CSV**.
- I imported the file named `Adventure Works sales dataset.csv`.
- I clicked **Load** to bring the data into Power BI.
  
  ![image](https://github.com/user-attachments/assets/a9b52c3b-f9f5-4a1b-a2e3-92ab5ba6b544)


**Why I did it:**
- This is the first step in working with data.
- Without importing the data, I wouldn’t be able to create any charts or dashboards.



## 🔷 Step 2: Create Interactive Filters (Slicers)

**What I did:**
- I clicked the **Slicer** visual from the Visualizations pane.
- I dragged the **Product Category** field into the slicer.
![image](https://github.com/user-attachments/assets/70edc77b-9d4b-4722-8579-8f11c7e9646a)

- I repeated the same steps to create another slicer for **Payment Method**.
![image](https://github.com/user-attachments/assets/97b0c9ab-e0cb-4b5e-9182-a838c1f8e8d7)
- I turned on and customized the **Title** for each slicer:
  - "Filter by Product Category"
![image](https://github.com/user-attachments/assets/d4fdc39e-dad4-4129-aeda-8ecca7b36f9a)

  - "Filter by Payment Method"
![image](https://github.com/user-attachments/assets/cef7b0aa-a62f-4d83-b862-04064a6cdda6)

![image](https://github.com/user-attachments/assets/57310275-89fd-40b4-aea1-668299f7df56)

- I moved both slicers to the **right side** of the report.

![image](https://github.com/user-attachments/assets/7cce64ea-dad5-4894-97d9-9a815ab35279)



**Why I did it:**
- Slicers help users interact with the report.
- They can filter data by product category or payment method to explore specific details.
- It makes the dashboard dynamic and easy to use.


## 🔷 Step 3: Create a Stacked Column Chart

**What I did:**
- I selected the **Stacked Column Chart** visual.
- I dragged the following fields:
  - **Order Total** → Y-Axis
  - **Product Size** → X-Axis
  - **Product Category** → Legend
- I updated the title using the Format tab to:
  - `Order Total by Product Size and Product Category for 2023`
![image](https://github.com/user-attachments/assets/5a475f56-dd5c-4bd9-9150-8d1c564cc337)
![image](https://github.com/user-attachments/assets/774431ce-987e-4cc7-80d5-81e20ffad291)

- I placed the chart on the **left side of the report area**, next to the slicers.

![image](https://github.com/user-attachments/assets/38a9d206-f961-4c56-824b-ae357e20e531)
**Why I did it:**
- This chart helped me compare how different product sizes and categories performed.
- It shows which categories had the most sales in each size group.



## 🔷 Step 4: Create a Donut Chart

**What I did:**
- I clicked on the **Donut Chart** visual.
- I dragged:
  - **Product Category** → Legend
  - **Order Total** → Values
- I changed the title to: `Order Total Share by Product Category for 2023`.
![image](https://github.com/user-attachments/assets/55ed7d96-7551-4345-a57e-6500a42683ff)
![image](https://github.com/user-attachments/assets/6a9bf90a-3f90-4c2b-ac72-562ace8f3dc9)


- I placed this chart **below the stacked column chart**.
![image](https://github.com/user-attachments/assets/3b9afa2a-641d-4015-922d-58ff269d579e)




**Why I did it:**
- Donut charts show the **percentage share** of each product category.
- It's useful for understanding how each category contributes to total sales.


## 🔷 Step 5: Create a Table

**What I did:**
- I selected the **Table** visual.
- I added the following fields:
  - **Product Name**
  - **Order Total**
- I moved the table **below the slicers** on the right side of the report.

  ![image](https://github.com/user-attachments/assets/94ef0a87-7c6d-495d-a2cb-9a21ae165cd4)



**Why I did it:**
- Tables show exact numbers.
- It helped me see the order total for each individual product in a clear way.

![image](https://github.com/user-attachments/assets/07c74dbb-073a-4eda-9471-fdd1f74c78d8)

![image](https://github.com/user-attachments/assets/8d579d14-62d0-4e3c-88a6-9730540ab3fd)

## 🧠 Conclusion – What I Learned

This exercise taught me how to turn raw data into clear and useful visualizations using Power BI. I learned how to:
- Import data,
- Create interactive slicers,
- Build charts like stacked columns and donuts,
- And display detailed information in tables.

Power BI made it easier to find insights and communicate results to the team. These visualizations can really help the company make better, data-driven decisions.

© 2025 Henok Tariku
