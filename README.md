<p align="center">
<img src="https://i.imgur.com/KuB3GsY.png" alt="Logo"/>
</p>

<h1 align="center">Ticket Lifecycle: Intake Through Resolution</h1>

Outlining the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Prerequisites and Installation</h2>

- _This Tutorial assumes that you went through the <a href="https://github.com/CarlosAlvarado0718/osTicket-PostConfig">"osTicket - Post-Install Configuration"</a> tutorial!!_

<h2>Lifecycle Stages</h2>

<h3>&#9312Opening a New Ticket as a Customer/Intake</h3>

>**Note***
>_Tickets are a Document that records the interactions on a support or service case_

- On the Web Browser (MicroSoft Edge), click on the End User Ticket Page (http://localhost/osTicket/).
- Click on `Open a New Ticket`

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/fde593c6-85bb-4687-bfe5-2d3253234a40)

- Enter **Karen's** Email Address and Full Name
- Enter any Help Topic or **Business Critical Outage**
- Click `Create Ticket`
- Type a Quick Header and a Short Summary under `Issue Summary`
  
  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/652d9eb2-2239-4ecf-bbdd-220443ffd581)

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/ba848e63-38a0-4b8a-b941-c971d837393d)

- Create two more tickets ranging from various importance for demonstration purposes

  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/7c1c805b-e47c-4e93-adbe-fc14f1f5dc0f)

![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/ff8bf36b-b457-4c92-9d53-5c4b0b77f5a3)

<h3>&#9313Assignment and Communication</h3>

>**Note***
>_Assigning a ticket means that the ticket must be routed to the appropriate agent or department to be able to act on it._

- On the Web Browser (MicroSoft Edge), go to the Help Desk Login Page (http://localhost/osTicket/scp/login.php).
  - Login using the **jane.doe@osticket.com** agent account
 
  ![image](https://github.com/CarlosAlvarado0718/osTicket_Lifecycle/assets/140138198/34c5b3e4-7bdd-4f81-a890-efc69f41fe01)

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

  <h3>&#9314Resolution</h3>

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
