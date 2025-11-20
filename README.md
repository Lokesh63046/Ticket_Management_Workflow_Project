**# 🎫 Ticket Management Workflow Automation
**
This project simulates a complete internal ticketing workflow system similar to Jira/ServiceNow using **Microsoft Excel**, with automated SLA tracking, a dashboard, and charts for operational insights.

This is a real-world style project suitable for Learning Operations, Support Ops, or Backend Operations roles.


**## ⭐ Project Highlights
**
 ✔ Built a **ticket tracker** with 100+ realistic support tickets  
 ✔ Implemented **SLA due dates**, **overdue detection**, and **priority escalation**  
 ✔ Designed **conditional formatting** for High Priority, Completed, Closed, and Overdue tickets  
 ✔ Added a full **Dashboard sheet** with KPIs and charts  
 ✔ Created a **professional PPT presentation** summarizing the workflow  
 ✔ Implemented formulas for end-to-end automation  


**## 📊 Dashboard KPIs
**
The Dashboard includes:

- **Total Tickets**
- **Overdue Tickets**
- **Completed Tickets**
- **High Priority Tickets**
- **Tickets With Comments**
- **Tickets by Agent**
- **Priority Breakdown**
- **Status Breakdown**

==>> All KPIs update automatically when new tickets are added.

**## 🧮 Excel Formulas Used
**
SLA Due Date: =IF(G2="","", G2 + (F2/24))

Overdue Check: =IF(G2="","", IF(AND(D2<>"Completed", D2<>"Closed", NOW() > H2), "Overdue", "On-Time"))

Improved Overdue Check: =IF(G2="","", IF(OR(D2="Completed", D2="Closed"), "On-Time", IF(NOW()>H2,"Overdue","On-Time")))

Auto Ticket ID : ="TCK-" & TEXT(ROW()-1,"000")

Dashboard Metrics:

Total Tickets:          =COUNTA(A:A)-1
Overdue Tickets:        =COUNTIF(J:J,"Overdue")
Completed Tickets:      =COUNTIF(D:D,"Completed")
High Priority Tickets:  =COUNTIF(C:C,"High")
Tickets With Comments:  =COUNTIF(K:K,"<>")

**📈 Dashboard Charts Included
**
Status Breakdown (Pie Chart)

Priority Breakdown (Pie Chart)

Overdue vs On-Time (Bar Chart)

Tickets by Agent (Bar Chart)



**🧩 Ticket Workflow
**
New → Assigned → In Progress → Completed → Closed
Each stage reflects the real ticket lifecycle in corporate systems like Jira or ServiceNow.

**📁 Folder Structure
**
Ticket-Management-Workflow/
│

├── Tickets.xlsx
├── Dashboard.xlsx
├── Presentation/

│   └── Final_Dashboard_Project_PPT.pptx

├── Screenshots/

│   ├── dashboard_main.png
│   ├── status_chart.png
│   ├── priority_chart.png
│   ├── overdue_chart.png
│   └── agent_chart.png

└── README.md

**🛠 Tools Used
**
Microsoft Excel

Conditional Formatting

Excel Charts

Microsoft PowerPoint

**🔗 How to Use
**
Open Tickets.xlsx

Add or modify ticket entries

Dashboard updates automatically

Charts and KPIs reflect new data instantly

👤** Developed By**

Bainaboina Lokesh

Ticket Management Workflow | Excel Dashboard | SLA Automation 

📍 Hyderabad, India 

🔗 www.linkedin.com/in/lokesh-bainaboina9848

**⭐ If You Found This Useful
**
Please ⭐ star the repository — it helps more people find resources like this!
