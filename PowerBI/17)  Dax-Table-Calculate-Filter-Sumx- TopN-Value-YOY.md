# Session 17) Dax-Table-Calculate-Filter-Sumx- TopN- Value-YOY
- https://youtu.be/upqexDr0c3c?si=oShu5gO8EklRVNzL

# There are 2 important  KPI (we can learn more in google):
- # YOY ⇒Year-on-year ratio
  - calculated using DAX by comparing a current period measure (e.g., Sales) against the same period last year using CALCULATE and SAMEPERIODLASTYEAR. 
- # MOM ⇒ month-on-month ratio

# Dax:
- # New table:
- <img width="380" height="227" alt="image" src="https://github.com/user-attachments/assets/ca08032a-5998-4b52-bc61-1c19f1c87faf" />
- Ex: Write a code to do some filter:
  -  region=North and product_name=Chayi and Revenue>200
  - Tbsale in north = Filter(tblSales,tblSales[Region]="North" && tblSales[Product Name]="Chai" && tblSales[Revenue]>200)

  - <img width="795" height="241" alt="image" src="https://github.com/user-attachments/assets/80443a5d-4ef7-4f2e-b597-68fdc93342f9" />
- && ⇒  And
- & ⇒ Concatenate

#  New Measure:
- # Ex:
-  write a code to write Null value for revenue column for  product_name=Oil:
- Cause we need a value ⇒ we have to use New Measure to return just one value:
- <img width="872" height="332" alt="image" src="https://github.com/user-attachments/assets/274fb0be-b375-44a2-9d70-77d46dbd1b9f" />
- Calculate ⇒ To apply a filter (category column) after performing the aggregate function  (without Calculate ⇒ it calculate sum of value without filter by category)
- filter ⇒ Create a virtual table with a special conditions ⇒ Like View in SQL
- on the  Sale_table , doing filter (category != oil)
- <img width="472" height="338" alt="image" src="https://github.com/user-attachments/assets/b3c0f932-872e-4220-85af-312ae9201ba3" />

- # We have to read this code from  right to left:
- <img width="895" height="152" alt="image" src="https://github.com/user-attachments/assets/1854a70f-cdb2-41d6-91ee-210dbfcb5d77" />

# SUM and  SUMX:
- 2 function sum  values  in column 
- SumX ⇒ we have to give a table (or Filter (Virtual table)) as a first  parameter and the Column as a second parameter
- <img width="681" height="328" alt="image" src="https://github.com/user-attachments/assets/4a4edd93-3fff-4671-af81-aaeef321ded3" />
- Sum ⇒ just sum on column and don't get table
- <img width="823" height="592" alt="image" src="https://github.com/user-attachments/assets/81899ed5-b1e0-4b99-adb2-6a46a9681b7f" />
<img width="405" height="314" alt="image" src="https://github.com/user-attachments/assets/d5e778dd-36d5-402a-a983-42e07e900530" />

# EX:
- write code with Dax code:
-  sale amount for region = North and south , other region=null
- Answer:
  - First way:
  - 1)Make Measure
  - 2)sum(revenue)
  - 3)make a filter on North and South
      - Filter(tbSale , Region in {“North”,”South”} )
  - 4)apply this Measure on All rows with⇒ Calculate
  - 5)add this measure to Table Visual as a column
   <img width="810" height="380" alt="image" src="https://github.com/user-attachments/assets/5a14b29e-2b84-4c8f-bf75-9025e1b8a848" />
- Sale amount for 5 Top product
- answer:
- <img width="611" height="621" alt="image" src="https://github.com/user-attachments/assets/44dd9880-0d0a-499e-aa31-32daa3075004" />


- # TopN:
<img width="772" height="101" alt="image" src="https://github.com/user-attachments/assets/50ac7ff6-a56a-46cf-94b2-4be57d1c9eb0" />
- # Value:
- <img width="767" height="190" alt="image" src="https://github.com/user-attachments/assets/dc7377da-4361-46c5-b0ab-34e75878d2c4" />
- <img width="717" height="662" alt="image" src="https://github.com/user-attachments/assets/952b086c-b56d-4733-b1bc-6b5a28cda9b1" />
- <img width="629" height="252" alt="image" src="https://github.com/user-attachments/assets/4cd3a854-f4c8-49a5-8c42-7fa32c843583" />
- <img width="669" height="574" alt="image" src="https://github.com/user-attachments/assets/b239e8b4-4825-4559-876a-7a8510a67fa1" />
- <img width="794" height="485" alt="image" src="https://github.com/user-attachments/assets/f4d0f491-1aed-4f4a-8cef-925c075f6c5d" />


- Sale amount for Green tea, Coffee, Chai , between 2014 until 2016
- <img width="1380" height="546" alt="image" src="https://github.com/user-attachments/assets/dd53ad80-b707-4fed-ba06-fb059cb00acc" />
<img width="756" height="275" alt="image" src="https://github.com/user-attachments/assets/444542e4-3b5a-42e7-afcd-aa5fbe1de669" />

- The best sale for each company  for product in these  group : 
  - Baked & Mixes
  - Beverages
  - Candy
  - Canned Meat
  - Condiments


