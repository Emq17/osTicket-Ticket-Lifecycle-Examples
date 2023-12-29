<p align="center">
<img src="https://i.imgur.com/KuB3GsY.png" alt="Logo"/>
</p>

<h1 align="center">Ticket Lifecycle: Intake Through Resolution</h1>

Outlining the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Microsoft Remote Desktop for Mac
- Internet Information Services (IIS)

<h2>Operating Systems</h2>

- Windows 10</b> (22H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Prerequisites and Installation</h2>

- _This assumes that you went through the <a href="https://github.com/Emq17/osTicket-Post-Installation-Configuration">"Administrative Post-Install Configuration"</a> demonstration walkthrough_

<h2>Lifecycle Stages</h2>

<h3>Opening a New Ticket as a Customer/Intake</h3>

>**Note***
>_Tickets are a Document that records the interactions on a support or service case_

- On the Web Browser (Microsoft Edge), click on the End User Ticket Page (http://localhost/osTicket/).
- Click on `Open a New Ticket`

![Screen Shot 2023-12-28 at 7 11 31 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/106098ad-4a49-4059-98ca-954f0fa1f546)

- Enter **Karen's** Email Address and Full Name
- Enter any Help Topic or **Business Critical Outage**
- Type a Quick Header and a Short Summary under `Issue Summary`
- Click `Create Ticket`

![Screen Shot 2023-12-28 at 7 13 55 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/bbe1a526-e48d-4665-97f7-c1304cffb8d7)

![Screen Shot 2023-12-28 at 7 15 38 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/deca1645-d88f-4444-945d-bae3a5c664dc)

- By clicking `Open a New Ticket`, create two more tickets with different Help Topics for demonstration purposes

![Screen Shot 2023-12-28 at 7 20 01 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/ffbc1e57-7f43-4d48-afc6-6eff567d54a7)

![Screen Shot 2023-12-28 at 7 22 15 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/4e3c0940-37ba-4dc7-956b-4f466c356d09)

<h3>Assignment and Communication</h3>

>**Note***
>_Assigning a ticket means that the ticket must be routed to the appropriate agent or department to be able to act on it._

- On the Web Browser (Microsoft Edge), go to the Help Desk Login Page (http://localhost/osTicket/scp/login.php).
  - Login using Admin account created from previous labs: **user_admin / Password1234** 
- As you can see in the Agent panel, there are all the tickets we have just created

![Screen Shot 2023-12-28 at 7 25 39 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/ed946472-658c-429a-8053-92fded677f6a)

- Go ahead and click on `Admin Panel` on the top right
- Click `Agents`
- Click `Jane Doe`

![Screen Shot 2023-12-28 at 7 28 39 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/17cefb71-1455-47c2-b629-b2e80dcacc86)






- Once logged in, you will see the existing tickets from the clients
   - Click on **Entire Mobile Online Banking is Down** Ticket

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/70dc9caa-544f-48ab-b57e-30b6533e7527)

>**Note***
>_As an Agent, You'll need to sort tickets by levels of impact, considering the entirety of the mobile online banking is being affected negatively, this will need to placed to the highest severity, alongside departments/teams to handle the situation ASAP!_

- Set `Priority` from Normal to **Emergency**
- Set `Department` to **System Administators**
- Set `Assigned to` **Jane Doe**
- Set the `SLA Plan` from Default SLA to **SEV-A**

 
![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/36cdaa8c-fdee-49f8-9e1e-297af89a7e9e)

- Under `Post Reply`, type **"Coordinating with Sys Admin Team to bring Mobile Banking back online"** 
- Keep the `Ticket Status` to **Open (current)**
- Click `Post Reply`

  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/62522582-372b-486a-9c25-0e28d3b3306b)

  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/7ad30087-eb97-44f6-affb-14be5fc6908d)

  <h3>Resolution</h3>

- Underneath `Post Reply`, type **Jerry from System Engineering found and corrected a failed load balancer. Mobile Banking should be back up momentarily.**
- Change the `Ticket Status` to **Resolved**

  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/03bedaf8-b113-4270-bf81-2d94df6c9cfe)

>**Note***
>_Once a ticket is resolved, it will be placed underneath the `Closed` tab_

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/e7139d33-ff53-41d1-819a-16dab281023b)

- Use your judgement to figure the rest of the ticket's `Priority`, `Department`, `Team`, etc

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/5a3d9344-5422-4a7e-b8df-f0dde16465f6)

---
<h1>COMPLETE! CONGRATS!!!</h1>

>**Note***
>_Rememeber to delete everything on Azure_
