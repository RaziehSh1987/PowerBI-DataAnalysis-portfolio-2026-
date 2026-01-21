# Session 8: Modeling, Fact and Dimension
https://youtu.be/gVmCt6Et2F0?si=o4vaBUj3eVRPlhoA

- In PowerBI:
  - We want to create a report
-In Excel (or in create table in power query):
  - Each employee how many calls they have yearly
<img width="207" height="199" alt="image" src="https://github.com/user-attachments/assets/ac864ffb-8a08-4e41-b311-362239c6c2ca" />

- And another table specifies each employee how much  they sale:

<img width="196" height="189" alt="image" src="https://github.com/user-attachments/assets/89920563-cf49-4139-b34c-b4961487eea3" />

- Ex: base on above table , create a report to show:
  <img width="257" height="93" alt="image" src="https://github.com/user-attachments/assets/d17a3236-b3cc-467d-9eb7-7f0dfc582869" />
- Employee - sale -phone call count
- And add slicer to filter year

# Fact:
- Each number that we want to show
- <img width="149" height="153" alt="image" src="https://github.com/user-attachments/assets/b8a9e48e-8713-4acc-9f37-0c78913ab881" />
- Like: it is just one number
<img width="273" height="190" alt="image" src="https://github.com/user-attachments/assets/1c89d9f0-f8d0-4e38-a805-de969f5b789c" />

# Dimension:
- The dimension of number that we want to see = the Filters that we want evaluate the Fact
- Like:  we show the sale amount with Year dimension. (this has 2 dimension)
- <img width="556" height="343" alt="image" src="https://github.com/user-attachments/assets/d05dd349-225f-4ddb-86f2-7affd63ef41b" />
- These are 3 sample dimension:
<img width="711" height="295" alt="image" src="https://github.com/user-attachments/assets/41a149d1-3ccf-4fa5-850b-fc47cb0d68ed" />

# Ex:
- we want create Fact and Dimension for class for attendance and absence:
- # Fact: 
  - aggregate function are fact
<img width="183" height="158" alt="image" src="https://github.com/user-attachments/assets/c4af415e-382a-4881-94e9-6c3acb7385e2" />

- # Dimension:
  - (when we can filter with different value)
<img width="636" height="238" alt="image" src="https://github.com/user-attachments/assets/f58942f0-23e0-45ee-b37e-a8a778d1237a" />
   
   - Number of absence base on ⇒ dimension are (date,age,education,name,..) => we can create different dimension for this fact(Number of absence)

# Ex : 
- in this table we determined the relation between each fact and dimension with 1 , if there isn’t relation it’s red
- <img width="801" height="107" alt="image" src="https://github.com/user-attachments/assets/b65b8dd8-cf32-4185-82c6-d9208b766c06" />

