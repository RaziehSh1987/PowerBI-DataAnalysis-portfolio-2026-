# Session 0 ) 
https://youtu.be/lNU6cc_1mzw?si=uE5zsCe89gmZQTwv

<img width="623" height="293" alt="image" src="https://github.com/user-attachments/assets/2bbc9446-34da-4021-9982-1a604e80d7fe" />

<img width="622" height="293" alt="image" src="https://github.com/user-attachments/assets/3f7579f4-9620-48b1-ba52-4a8d6608d29b" />
<img width="613" height="344" alt="image" src="https://github.com/user-attachments/assets/c6922bc6-6f97-4c8d-831d-4e6860d1efbc" />


In IRAN use ⇒ SSIS or power BI dataflows 
But
# In Canada use => python and airflow

Ex:
# Bulk load insert in sql:transfer all of the Data_base  at once
<img width="625" height="315" alt="image" src="https://github.com/user-attachments/assets/c51c701b-827e-4a87-a412-170e6ac6ccd7" />


# Incremental insert: conditional
<img width="627" height="244" alt="image" src="https://github.com/user-attachments/assets/6bb0395c-5a0d-441b-9ee6-dc3199c5462a" />


# Session 1) 
https://youtu.be/bzOq04sVB00?si=L81RJvSywbXOeBm5

<img width="613" height="354" alt="image" src="https://github.com/user-attachments/assets/5f396b88-a74e-4f35-aa64-ade83d01c75a" />
<img width="625" height="359" alt="image" src="https://github.com/user-attachments/assets/5803f431-d8b5-448e-8c81-c18d344777a1" />
<img width="627" height="364" alt="image" src="https://github.com/user-attachments/assets/5fe24a89-5ce7-4570-91f4-13d11c451f00" />
<img width="625" height="322" alt="image" src="https://github.com/user-attachments/assets/c455b176-c2ab-43b5-8972-df0d0ee2b729" />
<img width="621" height="339" alt="image" src="https://github.com/user-attachments/assets/4e1748cd-ac82-413a-b96b-e7f26a408aa6" />

- first of all we have to know, where the data_set is saved?
  - Excell,
  - CSV,
  - Sql ,..
<img width="583" height="364" alt="image" src="https://github.com/user-attachments/assets/4a66963b-a943-4aca-bfe5-79104a89f49c" />
<img width="586" height="327" alt="image" src="https://github.com/user-attachments/assets/ec7fa983-0e44-4a35-8edd-d0309fa8cba3" />

#PowerCI versions:
-  PowerBI RS version => Server version => which is version that administrators  open the browser for example Chrome and then connect to the powerBI Server and see the reports.
-  PowerBI Desktop

#ETL : 
-  Extract
-  Transform(cleaning)
-  load to PowerBI to show the reports

  # Learning order:
 Power query > Dax > Visualization > modeling

#Get data:
<img width="475" height="577" alt="image" src="https://github.com/user-attachments/assets/175be086-df95-40a7-976c-1e03d95a809e" />

- PowerBI > Get_data  >csv >
  - transform data
     - (open in power query then we can load into different view )
  - Load 
    - go directly to PowerBI (without power query)

# Power query:
-  On the table name > r.k > Enable node => if it is active => so the table shows in the power query but it doesn’t load 

-  Data source Setting: show all the files that is imported into power BI:
<img width="624" height="453" alt="image" src="https://github.com/user-attachments/assets/5d48b5f2-fa69-45fd-a801-a67ab3e02805" />

- we need two important information about each data source:
  - Path 
  - column  name ⇒ are important

# 📊 Data Types در Power Query (with simple example):
<img width="321" height="369" alt="image" src="https://github.com/user-attachments/assets/8ba38aea-ccf9-4f90-b11b-565629b47373" />

- 🟦 Text
  - String
Name
Country
Email
ProductName

- 🔢 Whole Number
  - Integer number (without Decimal❌)
Quantity = 5
Age = 32
OrderCount

- 🔢 Decimal Number
  - Its the most common type for Money 📌
Amount = 123.45
Price
Revenue
Percentage

- 💰 Fixed Decimal Number
    - For high-precision Currency / High accuracy /📌 Good value for money / ⚠️ Slower than Decimal Number / ✔️ For accurate financial reporting
Salary
Amount with money

- 📅 Date
    - just Date / without Time 📌
2024-06-01

- ⏰ Date/Time
    - Date and Time
2024-06-01 14:35

- 📌 Timestamp
  - ⏱ Date/Time/Timezone
  - 📌 When data comes from the API
2024-06-01 14:35 +03:30

- 🕒 Time
   - just Time
14:35:00

- 🔘 True/False
  - Boolean
IsActive
IsPaid

- 🧾 Binary
    - file
    - Image
    - PDF

- 🟪 Any
  - Undefined (Dangerous ⚠️)
  - 📌 means Power Query doesn't understand the type yet
  - ❌ Should not remain in the final model

- 🔑 Duration
Time difference
Session length


# Applied Steps:
There are 3 ways to Edit and View the Applied steps::
- APPLIED STEPS tab
 <img width="622" height="126" alt="image" src="https://github.com/user-attachments/assets/45146243-b7c1-410f-93ad-51bd21c5ac8b" />

- Function box
<img width="680" height="350" alt="image" src="https://github.com/user-attachments/assets/ed9d0032-bebb-4af2-ae93-867af05d515b" />

- Advanced Editor
<img width="476" height="723" alt="image" src="https://github.com/user-attachments/assets/2a4857b0-6da8-4638-913a-dda5994a619f" />


# Filter  and format the table cells:
<img width="566" height="591" alt="image" src="https://github.com/user-attachments/assets/199d0cb0-7487-4a13-886e-7c30c2efe8a8" />

- Transform : (filtering based on the Data Type):
    - Like: trim, UPPERCASE,.. For text
<img width="398" height="359" alt="image" src="https://github.com/user-attachments/assets/536a4014-e856-4a32-9066-8ff0c434ae28" />

- Change  or filter the row:
<img width="570" height="517" alt="image" src="https://github.com/user-attachments/assets/95f41885-9f33-4560-9c10-881249441b47" />

# Split column:
<img width="268" height="431" alt="image" src="https://github.com/user-attachments/assets/ccdba595-093e-4f77-95d7-db1a2d49fa44" />
<img width="594" height="196" alt="image" src="https://github.com/user-attachments/assets/9e0a84bb-f43d-4fb7-8558-e3b69600b569" />
<img width="368" height="703" alt="image" src="https://github.com/user-attachments/assets/3dff31f0-e8d2-4b1f-a217-90756d39f4e2" />
 
Filter all of the table:
![Uploading image.png…]()



