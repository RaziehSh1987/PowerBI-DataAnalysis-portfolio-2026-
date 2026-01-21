# Session 8: Modeling, Fact and Dimension
https://youtu.be/gVmCt6Et2F0?si=o4vaBUj3eVRPlhoA

- In PowerBI:
  - We want to create a report
-In Excel (or in create table in power query):
  - Each employee how many calls they have yearly

And another table specifies each employee how much  they sale:

Ex: base on above table , create a report to show:
  
Employee - sale -phone call count
And add slicer to filter year

# Fact:
Each number that we want to show

Like: it is just one number

# Dimension:
The dimension of number that we want to see = the Filters that we want evaluate the Fact
Like:  we show the sale amount with Year dimension. (this has 2 dimension)

These are 3 sample dimension:

Ex: we want create Fact and Dimension for class for attendance and absence:
Fact: 
aggregate function are fact

Dimension:(if we can filter with different value)

Number of absence base on ⇒ dimension are (date,age,education,name,..) => we can create different dimension for this fact(Number of absence)
# Ex : in this table we determined the relation between each fact and dimension with 1 , if there isn’t relation it’s red 

