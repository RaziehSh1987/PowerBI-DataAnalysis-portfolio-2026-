# session 14 : Tooltip-HierarchicalConcept-DrillThrough-ExportData
- Tooltip-DrillThrough-ExportData-hierarchical concept- Creating a dashboard on top of another dashboard, 
https://youtu.be/ierSMyKqpaY?si=TkxZXdm8yH7nT6aj
- This a  default Tooltip:
- <img width="444" height="301" alt="image" src="https://github.com/user-attachments/assets/9d524b17-0df7-4cb7-8e15-a05768627589" />

- But We want to show a Dashboard as a Tooltip when we move on specific part of another dashboard, like:
  - First, in the New Page > we have to set Canvas size on Tooltip size:
  - <img width="712" height="365" alt="image" src="https://github.com/user-attachments/assets/f2ec23e2-f8d5-4695-8fef-0398dd6b023c" />

  - We create our desire Tooltip like:
  - <img width="482" height="371" alt="image" src="https://github.com/user-attachments/assets/085dac7b-9df5-46b1-9205-34065df07062" />
  - We go to the main page that we want Show our tooltip on another dashboard:
  - Select visual that we want define Tooltip for its like Bar Chart:
  - In Visualization > Format visual tab > General >  tooltip > Type = Report page

    - # Note: we only see “Report Page” option ⇒ when we already created another page that contains a Tooltip otherwise  we see just Default option.
    - <img width="309" height="793" alt="image" src="https://github.com/user-attachments/assets/546787bc-e37d-4518-b054-8b405d3a25fc" />
    - Select the page that contains Tooltip:
    - <img width="247" height="335" alt="image" src="https://github.com/user-attachments/assets/80187373-5895-4fb7-b44b-e6879308fd44" />
    - Now, If we move on the bar we can see the other dashboard as a Tooltip:
    - <img width="636" height="384" alt="image" src="https://github.com/user-attachments/assets/5dffdc66-1cd2-4f45-bc2c-ded584e95d50" />

# Hierarchy investigation :
# 1) Using Line chart
- For example here we have 3 level (columns)
- <img width="557" height="233" alt="image" src="https://github.com/user-attachments/assets/c5aac7b6-b396-43b6-abde-e3dfad3b0bd0" />
- Ex: we create a line bar with x= Date table ( hierarchy) and y=revenue
<img width="1006" height="414" alt="image" src="https://github.com/user-attachments/assets/80a3729e-891d-41f7-9af1-b003b1aeb841" />
- #  What are these icons:
- <img width="637" height="612" alt="image" src="https://github.com/user-attachments/assets/727dd199-0388-4e1b-bfe0-5f9a17c37783" />
<img width="36" height="43" alt="image" src="https://github.com/user-attachments/assets/15f548d1-c37a-4d86-a834-93e9bc0f364a" />
<img width="909" height="468" alt="image" src="https://github.com/user-attachments/assets/088034de-ef46-4e6d-90ca-3592fd722c13" />

<img width="881" height="743" alt="image" src="https://github.com/user-attachments/assets/e88d70cf-29fb-44b1-a12b-40c42680e5a0" />
<img width="436" height="227" alt="image" src="https://github.com/user-attachments/assets/0bef54db-36c7-4c28-a272-29c4d3fc3c84" />

<img width="883" height="473" alt="image" src="https://github.com/user-attachments/assets/a9de55b3-abd7-4015-9b45-32a0acbe051c" />

# 2) using Clustered bar chart: 
<img width="297" height="451" alt="image" src="https://github.com/user-attachments/assets/95f6834b-fb91-41bb-873e-c12a5a17571e" />

# Note:
-  when click on  this icon <img width="68" height="88" alt="image" src="https://github.com/user-attachments/assets/5c1fadcc-b38d-4e2e-9c41-83793801d4bb" />
   ⇒ This sum all of the category that we put in x-axis  (here we have only one Beverage on the chart
   <img width="902" height="563" alt="image" src="https://github.com/user-attachments/assets/d7d29bd2-5e89-4322-a59b-1ac57bea6e4d" />
   - But with this icon  ⇒ it categories into the 2 category (because we added 2 element in x-axis) (here we have 2 category on the chart), like:
   - <img width="797" height="705" alt="image" src="https://github.com/user-attachments/assets/31d88b3a-8bd3-4215-b230-cd94596f14ef" />

  # Drill mode:
  - <img width="731" height="137" alt="image" src="https://github.com/user-attachments/assets/7c94a030-850d-47b2-80bc-c924fdb73851" />

  <img width="835" height="490" alt="image" src="https://github.com/user-attachments/assets/4338910c-725c-4033-9025-bf7e4ef5b1d1" />
  - With click on this:
<img width="823" height="390" alt="image" src="https://github.com/user-attachments/assets/d24a58a1-6722-4b16-9329-ad443d410919" />
- We will see its subcategories::
- <img width="832" height="434" alt="image" src="https://github.com/user-attachments/assets/208bdcca-1e82-4146-a613-bb4b98c948f1" />
<img width="786" height="444" alt="image" src="https://github.com/user-attachments/assets/5994d95f-4456-4bcb-a2b4-58add537fad0" />

- Then  save as .csv file:
- <img width="616" height="489" alt="image" src="https://github.com/user-attachments/assets/6d44488c-5c2d-4ca3-9e3d-7880564cf219" />
# Show table:
<img width="563" height="336" alt="image" src="https://github.com/user-attachments/assets/5897cf96-8d24-4e1b-aed0-5889b78da289" />

<img width="869" height="490" alt="image" src="https://github.com/user-attachments/assets/6e43d126-97f7-4e76-a3e0-0b8c37ed3ba7" />

# Analyze: 
- We can see the different dashboard that it created and we can import it in our dashboard:
- R.k on the chart:
- <img width="869" height="290" alt="image" src="https://github.com/user-attachments/assets/1f1be0f1-79ad-470c-a349-1cf36ac1e334" />
- See the results
- <img width="637" height="675" alt="image" src="https://github.com/user-attachments/assets/5cf41b49-68df-4994-99b7-7aaab4ff634e" />
- We can add to our dashboard by click on :
- 
- <img width="405" height="347" alt="image" src="https://github.com/user-attachments/assets/e2bd41d8-1ebc-4155-8f52-93e1a937a428" />
<img width="825" height="587" alt="image" src="https://github.com/user-attachments/assets/ccf1645d-8401-4b55-b909-0e5e06a8e81e" />

# Customize Drill through:
- We want to show the filter result  in different page based on specific element (like Product name)  by R.K on the chart’s element and select " Drill  through " :
- <img width="589" height="452" alt="image" src="https://github.com/user-attachments/assets/72df2856-cac7-4bc9-9af5-be0256dd09a6" />
- For example:
- <img width="857" height="537" alt="image" src="https://github.com/user-attachments/assets/ce9ea157-15ef-4a6b-97d0-af4126abcf80" />
- Then we can see the details of that filter:
<img width="863" height="488" alt="image" src="https://github.com/user-attachments/assets/07be244b-69ed-4e2c-a89f-22d4f2e9299a" />
- Select destination table
- We enable and set Drill through = Category field  for this bar chart  (to drill (filter) each bar based on Category)

- # Drill-through field must be on the target page
- Go to the destination page (the page you want to drill INTO).
  - In Visualizations → Drill-through
  - You must drag a field (e.g. Customer, Country, Date, Product)
  - 
# Note:
- # You must right-click the same field
- On the source page, you must:
    - Right-click a data point
    - That data point must contain the exact same column (or a column related through model)


- Example
  - If drill-through uses:
<img width="304" height="45" alt="image" src="https://github.com/user-attachments/assets/9b0115a3-882d-4281-b464-becbde6fb4fe" />

- Then right-click must be on:
    - A visual grouped by CustomerName
       -  ❌ Not on totals
       - ❌ Not on unrelated fields
      <img width="233" height="528" alt="image" src="https://github.com/user-attachments/assets/342bbb7a-c0c6-493c-bc6d-83f804236cf0" />

   - I can come back to upper level by click on ( <img width="104" height="127" alt="image" src="https://github.com/user-attachments/assets/0303d78e-0062-419f-842b-969c3616d3c0" />
 + ctrl)
   - <img width="642" height="657" alt="image" src="https://github.com/user-attachments/assets/17a6e50e-2aed-4521-b5b8-f69de7bd807f" />

   <img width="897" height="298" alt="image" src="https://github.com/user-attachments/assets/c9ab1c7e-c0c2-421c-bca1-d36223459cc2" />















































