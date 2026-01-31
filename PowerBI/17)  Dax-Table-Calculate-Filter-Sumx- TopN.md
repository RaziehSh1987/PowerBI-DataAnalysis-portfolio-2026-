# Session 17) Dax-Table-Calculate-Filter-Sumx- TopN
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
  - 2) sum(revenue)
  - 3) make a filter on North and South
      - Filter(tbSale , Region in {“North”,”South”} )
  - 4) apply this Measure on All rows with⇒ Calculate
  - 5) add this measure to Table Visual as a column
   <img width="810" height="380" alt="image" src="https://github.com/user-attachments/assets/5a14b29e-2b84-4c8f-bf75-9025e1b8a848" />
- Sale amount for 5 Top product

# TopN:
<img width="772" height="101" alt="image" src="https://github.com/user-attachments/assets/50ac7ff6-a56a-46cf-94b2-4be57d1c9eb0" />
 <img width="644" height="643" alt="image" src="https://github.com/user-attachments/assets/84628fad-73bd-4a41-b49a-8ec29b53adab" />
 
- Sale amount for Green tea, Coffee, Chai , between 2014 until 2016
- The best sale for each company  for product in these  group : 
  - Baked & Mixes
  - Beverages
  - Candy
  - Canned Meat
  - Condiments


