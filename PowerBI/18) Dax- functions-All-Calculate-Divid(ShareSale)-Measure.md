# Session 18) Dax- functions-All-Calculate-Divid-Measure

# Calculate:
<img width="507" height="67" alt="image" src="https://github.com/user-attachments/assets/ee6b9926-521c-409f-aff1-1f49ae71987a" />
- Calculate have 2 part:
  - Expression: sum,count,ave,..
  - Filter:table,True/false,..

<img width="760" height="605" alt="image" src="https://github.com/user-attachments/assets/5d75a7fa-29e4-45d2-b29e-6a738d4123ca" />

- We have 2 Filter type:
    - Direct
    - Indirect : like Revenue column   in below example that has indirect filter with Sum function.
    - <img width="1401" height="666" alt="image" src="https://github.com/user-attachments/assets/8c8bd845-e04a-417e-9fa6-2e4d4a9c04ef" />

- If we write below code, the result is :
- <img width="557" height="520" alt="image" src="https://github.com/user-attachments/assets/35f3c702-58ff-4cae-a452-f9891cf560e1" />
- But with ⇒ Calculate(sum()) ⇒ it calculate total sum and put it in front of each category
- <img width="1377" height="630" alt="image" src="https://github.com/user-attachments/assets/cc468c1d-202d-4c0d-9349-1589536c3864" />
- Now, we want doing a change:
    - Instead of sum(revenue) for each category ⇒ write total sum of revenue (like 1.56)  in front of each category

- # All():
- <img width="842" height="367" alt="image" src="https://github.com/user-attachments/assets/fd0c8e83-8835-4626-950f-6bcd838868fb" />
- Don’t filter the expression in Calculate(sum), by this column (tbsales[category]) that I write in ALL()
- <img width="789" height="228" alt="image" src="https://github.com/user-attachments/assets/774f9e18-9aee-49aa-a92d-37c940fe8d0f" />
<img width="863" height="803" alt="image" src="https://github.com/user-attachments/assets/4161011f-f926-4422-a11b-c7955a25a667" />
- For example in below code⇒ I mention that don’t filter(indirect) on sum(revenue) by category ⇒ while I add the “customer” column not “category” column
- <img width="1555" height="579" alt="image" src="https://github.com/user-attachments/assets/bfb301c1-f70c-4f0b-9802-3d2278df7e94" />
- But if I add “category” column⇒ sum(revenue) will be filter by category⇒ because I write All(“category”)
- <img width="1436" height="639" alt="image" src="https://github.com/user-attachments/assets/250b9914-0326-4633-9fc9-b4aadfe22ea6" />
- All() ⇒ can get one column or more than one column or table:
  - Means⇒ when you see every column in this table, don’t do filter
  <img width="1503" height="595" alt="image" src="https://github.com/user-attachments/assets/7f90c606-1e68-41a2-8c3b-186187d72601" />

# Ex:
- <img width="397" height="119" alt="image" src="https://github.com/user-attachments/assets/1a7103f5-a41e-43bb-948a-70d06631e500" />
- Create this table with DAX :product name / sale amount/Sales share
- Answer:
  - Make a Measure:
  - # Divide or "/":
  - 12/4 or divide(12,4)
  - <img width="643" height="145" alt="image" src="https://github.com/user-attachments/assets/f56f8c39-22bc-4d7b-a19a-68d949783f38" />
  - Add ⇒ Table visual with this columns ⇒ product_name / sum(revenue) / SaleShare
  - Select SaleShare > format menu >   format=percentage
  <img width="1219" height="641" alt="image" src="https://github.com/user-attachments/assets/88612966-4d64-46fb-8cce-968cbe887ee8" />








