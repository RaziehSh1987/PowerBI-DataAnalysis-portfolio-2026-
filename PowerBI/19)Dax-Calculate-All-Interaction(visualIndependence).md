# Session 19)  - Dax-Calculate-LeftToRight-All(= remove filter)-Edit Interaction(visual Independence)-
https://youtu.be/0WauCkI1O9k?si=pweJDszTx9CLibvP

# Calculate:
- Read from Left to Right:
- <img width="887" height="302" alt="image" src="https://github.com/user-attachments/assets/5bea9c27-a7b3-434c-a708-3e9a5a6be6da" />
- First ⇒ sum(Revenue)  
- Then⇒ apply this filter (category=”ada”) on the result of first step =is like Slicer
- like:
- <img width="1374" height="699" alt="image" src="https://github.com/user-attachments/assets/9ae73933-2049-400a-99a2-5402e1972cde" />

# All:
- Is like Remove Filter based on X
- Like: in below measure we say⇒ sum(revenue) ⇒ then : if you see Category column, don’t filter by “Category” column
- <img width="1512" height="773" alt="image" src="https://github.com/user-attachments/assets/19d2da91-e3ad-46ae-96b8-18e5a4d14991" />

# EX: write a Dax code to show the Share Sale based of Year:
- <img width="854" height="381" alt="image" src="https://github.com/user-attachments/assets/72277167-3899-4231-8dd9-29aeecdb95db" />
- Answer:
- <img width="772" height="192" alt="image" src="https://github.com/user-attachments/assets/c7989fd6-3a4a-45da-9b94-1b43d9bcda45" />
- This code equal to : Percentage of grand total
- <img width="682" height="306" alt="image" src="https://github.com/user-attachments/assets/e1522c6d-0f98-49d7-8547-e1fe4da43afc" />
- <img width="1643" height="705" alt="image" src="https://github.com/user-attachments/assets/9ae1a3a8-55aa-4ccb-ae8c-3cb40427b7cb" />
- If I put Legend=Category ⇒ it shows my Visual for all categories
- <img width="1713" height="757" alt="image" src="https://github.com/user-attachments/assets/ef5c8af4-2ffe-4fa7-b618-3e20f58a1be5" />

# Edit interaction: 
- How to make two visuals independent in Power BI
- <img width="1212" height="586" alt="image" src="https://github.com/user-attachments/assets/f5b39285-54de-41a2-b2ea-74c37f000828" />
<img width="682" height="659" alt="image" src="https://github.com/user-attachments/assets/c2d07fb0-d88e-47d7-9cd7-ae01663788c0" />

# All Except:
- filter Only with this element
- <img width="1212" height="178" alt="image" src="https://github.com/user-attachments/assets/9d4767ae-e5b9-4a41-ba6a-a6c0ca71f3ae" />
- This measure will be filter only with Category field
- <img width="1570" height="612" alt="image" src="https://github.com/user-attachments/assets/0cd73f3a-bb0e-4e36-a3a2-b6853e525041" />
# AllNoBlankRow:
- Filter the table that doesn’t have NULL value
- <img width="759" height="167" alt="image" src="https://github.com/user-attachments/assets/6b60104e-b9f6-4bc9-9252-46b4a441a1bb" />

# AllSelected:
- Returns all the rows in a table, or all the values in a column, ignoring any filters that might have been applied inside the query, but keeping filters that come from outside.
- <img width="784" height="485" alt="image" src="https://github.com/user-attachments/assets/f536b120-e6f4-4475-be91-b5e6419131f7" />
























