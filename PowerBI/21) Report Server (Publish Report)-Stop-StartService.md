# Session 21) Report Server (Publish Report)-Stop-Start Service-
- https://youtu.be/6P539N_X4mY?si=Yyhy_mImt3tA6ZnR

- We use Report server to Publish our Report to use by clients

# Download Report Server Application:
https://www.microsoft.com/en-us/download/details.aspx?id=105944
<img width="696" height="488" alt="image" src="https://github.com/user-attachments/assets/b1b509fb-d8b4-4b3a-97ab-f876487b35da" />
- Select PowerBIReportServer:
- <img width="723" height="439" alt="image" src="https://github.com/user-attachments/assets/93177a5e-f764-4efa-a187-dce5c44cfd1f" />
- Install > select Developer in the menu:
- <img width="677" height="566" alt="image" src="https://github.com/user-attachments/assets/64d52e1c-a8f9-43eb-92b8-1b820d7c94b4" />
<img width="676" height="59" alt="image" src="https://github.com/user-attachments/assets/16e5cdac-2b00-4c80-9db1-083af332215d" />
- Now we need to configure Report Server and connect it to our server:
- <img width="663" height="508" alt="image" src="https://github.com/user-attachments/assets/7b9f0c0f-97af-45f1-b7ba-3a30434acbc4" />
- If we work on our laptop⇒ we connect to our server ex: RaziLaptop 
- else, if we want to connect to the specific Server ⇒ we have to write Server IP 
- Click on Connect button
- We can Stop or Start the service that run Report server in this part.
  - If we see the error on the report (in the future) ⇒ the server is stoped, we can come here and start it again
<img width="806" height="618" alt="image" src="https://github.com/user-attachments/assets/455b65db-5cb0-4ac6-8af4-1bf7c5c43380" />
- Now, we determine , who can connect to report server ans see the dashboard:
  - Network Service: al of the user in our same network can connect to our report server with their User and password
  - Virtual Service Account: only the user who have user ID of Report server can connect and see our report
  - <img width="591" height="104" alt="image" src="https://github.com/user-attachments/assets/08851aa6-8010-4220-a9de-6d7b80a1005e" />
  - Use another account: we can create an account for user who is in our network
  - <img width="413" height="33" alt="image" src="https://github.com/user-attachments/assets/755b670b-833a-40ba-8e0e-736412983c70" />
  <img width="801" height="664" alt="image" src="https://github.com/user-attachments/assets/988fb983-0626-4c88-a95c-1a5ff1718d63" />
  -  Apply ⇒ to save configurations
  -  Now, we can setup the directory name/ip address/port of Link  that client want to connect tour dashboard via that link:
  -    <img width="693" height="90" alt="image" src="https://github.com/user-attachments/assets/786faa41-c14e-4217-80e1-e407208a77f7" />
  - The best setting is  below  setting (but if the port was closed you can ask of network team and change the port)
  - <img width="827" height="408" alt="image" src="https://github.com/user-attachments/assets/7e31efca-8e93-4411-9737-6a591895ee13" />
  - We Can define  where  save all of the changes related to our dashboards which in on the report server:
  - <img width="814" height="384" alt="image" src="https://github.com/user-attachments/assets/b3e7d6f6-b70f-4607-a30e-4bbb2e75f769" />
  - Click on Change Database >
  - <img width="808" height="690" alt="image" src="https://github.com/user-attachments/assets/7dbdb770-617a-408d-a4f8-4a49cf5c2c06" />
  - <img width="775" height="402" alt="image" src="https://github.com/user-attachments/assets/2bcbdc8c-632a-4383-9db2-bc4e20a56f53" />
- Create database in current user (our laptop) or another server ⇒ I selected current user > Test connection
- Next
- <img width="553" height="137" alt="image" src="https://github.com/user-attachments/assets/36e749da-b00e-4e0b-bf95-b3b6b537b72e" />
- Select type:
- <img width="774" height="223" alt="image" src="https://github.com/user-attachments/assets/72b8ccc1-9cea-4aa2-abb9-e416b573af91" />
- Next > finish
- This is final step and we want set the URL name that user want use that:
- <img width="868" height="180" alt="image" src="https://github.com/user-attachments/assets/0e88c879-e672-4f0c-a198-8bbc82eeb017" />
- In Virtual Directory⇒ we write the name that want add at the end of the URL link.

# Upload our Dashboard on the Report Server that we created:

