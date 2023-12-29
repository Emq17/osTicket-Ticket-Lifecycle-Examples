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
  - Login using the **jane.doe** agent account you had created in the last lab

![Screen Shot 2023-12-28 at 7 51 39 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/27c544ff-4bfd-4445-bcbf-66dd786abe34)

- Once logged in, you will see the existing tickets from the clients
   - Click on **"Entire mobile online banking is down"** Ticket

![Screen Shot 2023-12-28 at 7 52 12 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/f28e328b-a2e8-47ff-a58d-09179c9735a4)

>**Note***
>_As an Agent, You'll need to sort tickets by levels of impact, considering the entirety of the mobile online banking is being affected negatively, this will need to placed to the highest severity, alongside departments/teams to handle the situation ASAP!_

- Let's rework this ticket and pretend as if we are the Queue Manager making sure this ticket is proper
  - Set `Priority` from Normal to **Emergency** by clicking on `Normal` which will let you update it
  - Set `Department` to **System Administators**
  - Set `Assigned to` **Jane Doe**
  - Set the `SLA Plan` from Default SLA to **SEV-A**
    - In some organizations, the customers gets to choose the severity of the ticket which means that sometimes instead of raising the priority of one, you may have to instead put it lower regarding the actual issue

![Screen Shot 2023-12-28 at 8 01 03 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/9296311e-71d1-4033-a259-6571236009ea)

![Screen Shot 2023-12-28 at 7 57 22 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/d63da2ff-04e6-4aa3-ab64-30b09fdfb3d4)

![Screen Shot 2023-12-28 at 8 03 14 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/dd70d8f1-96eb-465f-8c93-6ba3307de9c0)

- Under `Post Reply`, type **"Coordinating with Sys Admin Team to bring Mobile Banking back online"** 
- Keep the `Ticket Status` to **Open (current)**
- Click `Post Reply`

![Screen Shot 2023-12-28 at 8 06 04 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/1fdef569-5b00-48f4-a45a-5cd0dcca29d5)

![Screen Shot 2023-12-28 at 8 06 29 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/d7759277-2036-4cad-9b4b-2807087b6622)

- Click `Tickets` tab up top
- Now you can observe how the ticket has been updated 

![Screen Shot 2023-12-28 at 8 08 34 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/9471cde6-37b2-44cd-bbf3-2cb76e77396b)

  <h3>Resolution</h3>

- Go back inside the ticket and lets pretend that we somehow fixed the issue 
- Underneath `Post Reply`, type **"Jerry from System Engineering found and corrected a failed load balancer. Mobile Banking should be back up."**
- Change the `Ticket Status` to **Resolved**

![Screen Shot 2023-12-28 at 8 12 36 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/83decac1-32dd-485c-a7b3-7c9cefe3256c)

>**Note***
>_Once a ticket is resolved, it will be placed underneath the `Closed` tab_

- So go ahead play around with everything and repeat these steps for the rest of the other tickets.
- You may notice that if you assign any tickets to "John Doe" and try to resolve them by logging into him (john.doe/Password1234), due to the "View only" access we've given him, you are not able to close them out. All you have to do is sign back into your admin account (user_admin) then update the settings giving him the "Supreme Admin" role.

![Screen Shot 2023-12-28 at 8 13 28 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/3100dc47-cacf-4440-b683-00bf76f769e0)

![Screen Shot 2023-12-28 at 8 15 22 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/546e3bf5-37a1-4345-8031-66ab9f12e323)

- Within these tickets, you can get a glimpse of the overall history of what was done to it

![Screen Shot 2023-12-28 at 8 17 57 PM](https://github.com/Emq17/osTicket-Ticket-Lifecycle-Examples/assets/147126755/c2a0a251-b930-4edf-a867-0535655a3f70)

# I hope this has given you a deeper understanding of osTicket

- Expanding on the last point I made, what you can do to become better than average at your job is, in your free time, to simply look through as many past tickets as you can to get a sense for the type of problems of what happened in the environment so that you are much better equipped on fixing these overall issues
- This advice should help many juniors starting from scratch or people who are nervous that are just starting out on a team to get ahead

---

<h3 style="text-align: center;"><i>As standard practice, verify your Azure resources/virtual machines, then delete the ones you don't need to prevent excessive utilization of subscription credits or the loss of money</i></h3>




  
