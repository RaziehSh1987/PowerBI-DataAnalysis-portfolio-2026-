
# Session 9: Fact-Dimension-DataWareHouse-BusMatrix
https://youtu.be/mwUW-DTIYAo?si=JH4MM5bud1VI-GG2
# Data Warehouse Bus Matrix :
- A “Data Warehouse Bus Matrix” describes the high-level design of a Data Warehouse. At a glance, it shows all the facts and dimensions of a data warehouse and their relationships in a table-like ‘matrix’
A “Data Warehouse Bus Matrix” describes the high-level design of a Data Warehouse. At a glance, it shows all the facts and dimensions of a data warehouse and their relationships in a table-like ‘matrix’. It’s useful as a tool to design, plan, estimate and communicate your data warehouse.

like:
<img width="753" height="337" alt="image" src="https://github.com/user-attachments/assets/489301c8-a41f-4276-9b3c-702e73000c20" />
- or
<img width="794" height="315" alt="image" src="https://github.com/user-attachments/assets/e38d8047-5cf2-4f12-b877-a8571c288812" />


# Ex: 
-  # Fact (Number) and Dimension (Filter) →for   Production
  - Using data warehouse Bus_Matrix to specifies Fact and DImension and relation between them:
<img width="564" height="224" alt="image" src="https://github.com/user-attachments/assets/134c11b2-0bd5-4f13-abb0-b181714c94c0" />

- Design Tables:
  - We want create the first Fact 
    - we use all of the related Dimensions as its columns + fact value(count)
    - We use this format to name the table ⇒ 
    - # FACT-tableName
    - # DIM-tableName
<img width="490" height="161" alt="image" src="https://github.com/user-attachments/assets/cb49f0a0-4fb0-466d-b18d-49a00866d220" />

- Then we create the rest facts
- Now, we create all of the Dimension tables, like:
 <img width="478" height="278" alt="image" src="https://github.com/user-attachments/assets/7721e878-08b9-40b5-beb6-2acc2ae41dfc" />
 
- We create a connection between shared columns for all dimensions with related Fact:
- <img width="762" height="400" alt="image" src="https://github.com/user-attachments/assets/f7577c9c-974d-4482-a1f6-5b3f0e9e558e" />

- We add another fact with their relations:
- <img width="755" height="264" alt="image" src="https://github.com/user-attachments/assets/5a938367-632e-45a4-a8e7-519a0a1b05a2" />


# Ex:
- create a table as PhoneCall:
<img width="786" height="229" alt="image" src="https://github.com/user-attachments/assets/a0ec4e72-be6b-4675-9965-b9061272c748" />
<img width="781" height="580" alt="image" src="https://github.com/user-attachments/assets/a83f4a69-f3a8-48ba-9caf-8273d0d25503" />
- We want to create this dashboard:
- <img width="734" height="406" alt="image" src="https://github.com/user-attachments/assets/4b00a34c-279e-44ab-8363-e3bb95cdd8dc" />
- We have 3 Filters for Date , Province , Sailer
- Left Sailer table ⇒ contains Sale and Target
- Right Sailer table ⇒ contains Sale and Call count
  
# Answer:
- We have to create Dimensions (the tables which we want make the  Filters based on them ):  Date-Saler-Province
<img width="630" height="748" alt="image" src="https://github.com/user-attachments/assets/62bcd3b2-a045-492f-bb58-ed9c4ba75453" />
  - So we have these tables:
<img width="253" height="254" alt="image" src="https://github.com/user-attachments/assets/5b578757-0df8-4696-a608-de88979daa28" />

   - We create the relations:
   - <img width="774" height="500" alt="image" src="https://github.com/user-attachments/assets/ac7a1b51-5f3c-4249-a622-3eae2e3cbbc6" />
   - Note: the Fact doesn’t filter the Dimension but the  Dimension filter the fact⇒ so the relationship is One way
<img width="705" height="711" alt="image" src="https://github.com/user-attachments/assets/fdb1b522-12af-46df-b0e9-f64c943d87de" />
- Enabling Data Label for each column: 
<img width="506" height="548" alt="image" src="https://github.com/user-attachments/assets/07adeb85-4ab7-4452-827f-a4ae36ebe7e2" />
- Note: when we filter the province, it doesn’t affect on the target fact ⇒ because target table doesn’t have the province column ⇒ so there isn’t relation between 2 tables


