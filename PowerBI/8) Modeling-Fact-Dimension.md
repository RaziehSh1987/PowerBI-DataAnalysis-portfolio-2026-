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

Ex:in my tables ⇒
<img width="462" height="217" alt="image" src="https://github.com/user-attachments/assets/740b0726-613d-4582-9d64-94ad8e9b26fb" />

 - sales and count_activity are => fact (show these data)
- Em , date => dimension (Filter by these data)
- 
- Modeling : If I want make relation between 2 tables without merge(join) function⇒ I have to Model the table:
  - I have to create the separate tables for each shared dimension like: em and date ⇒we have to  REMOVE DUPLICATE  (because it’s as a table key for relation)
<img width="607" height="589" alt="image" src="https://github.com/user-attachments/assets/f524799f-9c57-41e1-8536-ae8e674c6634" />

- Then go to the Model view  and make connection between them
- <img width="298" height="373" alt="image" src="https://github.com/user-attachments/assets/033b58a6-5849-46f6-bd8e-4052660a3476" />
<img width="812" height="297" alt="image" src="https://github.com/user-attachments/assets/e453745a-f0da-4c61-be05-53d1ff147fe0" />

- Now, in PowerBI we can create our report
- <img width="341" height="345" alt="image" src="https://github.com/user-attachments/assets/b96aa22d-5bbd-403c-a802-be4a85ea693c" />


# Modeling:
-<img width="590" height="296" alt="image" src="https://github.com/user-attachments/assets/e0f9ac00-e102-4fa3-898f-b1675313bca1" />

- <img width="783" height="624" alt="image" src="https://github.com/user-attachments/assets/2dc0fba6-5ec0-4b3f-a6d9-f91067f40691" />

- Many to one (*:1)
- One to one (1:1)
- <img width="627" height="170" alt="image" src="https://github.com/user-attachments/assets/bd9bd568-035d-4271-baee-e6810e6a6068" />
  - For each (one) class ⇒ we have one prof
- One to many (1:*)
- <img width="227" height="380" alt="image" src="https://github.com/user-attachments/assets/6fd351aa-10b0-40a3-956c-5d431a793966" />

- Many to Many (*:*)
  - We don’t have in PowerBI ⇒ we have to break to *:1 or 1:*
  - <img width="214" height="370" alt="image" src="https://github.com/user-attachments/assets/96ed73f7-772e-4d34-bd68-2cd3a706edee" />
- We can disable the relation by double click on the relation line  and deactivate below checkbox
<img width="341" height="149" alt="image" src="https://github.com/user-attachments/assets/51890963-1314-4a05-b102-19fca6b4b818" />
- I have a single or both relation in Cross filter direction drop down menu:
<img width="698" height="660" alt="image" src="https://github.com/user-attachments/assets/f1f5852d-0059-450a-9ff5-ef3cce6d46d6" />
- If I enable Both filter direction for Phone_call table: 
  - I can filter the Phone table and sale table (which are connected by the dimension ) in 2 Direction:
  - Click on relation:
  - <img width="646" height="274" alt="image" src="https://github.com/user-attachments/assets/7037b408-755b-47fb-9942-70b090c9fe45" />
- Select Both:
- <img width="488" height="220" alt="image" src="https://github.com/user-attachments/assets/583742fe-f430-4f25-908f-ddb8a0fff29e" />
- Now we can active 2 direction filter between tables:
<img width="681" height="225" alt="image" src="https://github.com/user-attachments/assets/3f4b5ae5-a209-473c-a58e-aa28127a4cda" />


https://youtu.be/gVmCt6Et2F0?si=fkYkRpey2MV1GPSw


