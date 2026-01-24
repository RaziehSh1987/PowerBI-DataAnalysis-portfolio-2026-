
# Session 9: Fact-Dimension-DataWareHouse-BusMatrix
https://youtu.be/mwUW-DTIYAo?si=JH4MM5bud1VI-GG2
# Data Warehouse Bus Matrix :
- A “Data Warehouse Bus Matrix” describes the high-level design of a Data Warehouse. At a glance, it shows all the facts and dimensions of a data warehouse and their relationships in a table-like ‘matrix’
A “Data Warehouse Bus Matrix” describes the high-level design of a Data Warehouse. At a glance, it shows all the facts and dimensions of a data warehouse and their relationships in a table-like ‘matrix’. It’s useful as a tool to design, plan, estimate and communicate your data warehouse.
like:

- or


# Ex: 
- Fact (Number) and Dimension (Filter) →for   Production
  - Using data warehouse Bus_Matrix to specifies Fact and DImension and relation between them:

- Design Tables:
  - We want create the first Fact 
    - we use all of the related Dimensions as its columns + fact value(count)
    - We use this format to name the table ⇒ 
    - FACT-tableName
    - DIM-tableName

- Then we create the rest facts
- Now, we create all of the Dimension tables, like:
 

- We create a connection between shared columns for all dimensions with related Fact:

- We add another fact with their relations:

# Ex:
- create a table as PhoneCall:



- We want to create this dashboard:

- We have 3 Filters for Date , Province , Sailer
- Left Sailer table ⇒ contains Sale and Target
- Right Sailer table ⇒ contains Sale and Call count
  
# Answer:
- We have to create Dimensions (the tables which we want make the  Filters based on them ):  Date-Saler-Province



  - So we have these tables:

   - We create the relations:
   - Note: the Fact doesn’t filter the Dimension but the  Dimension filter the fact⇒ so the relationship is One way

   - Note: when we filter the province, it doesn’t affect on the target fact ⇒ because target table doesn’t have the province column ⇒ so there isn’t relation between 2 tables


