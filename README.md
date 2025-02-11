# Customer Retention Analysis

## Problem statement
Customers in the telecom industry are hard-earned:Telecom company don’t want to lose them
•	The retention department is here to get customers back in case of termination.
•	To know in advance who is at risk.
•	To know more about customers

## Project Goal
•	Create a dashboard using KPIs that reflect customer demographics and insights.
•	Explain findings from dashboard and suggest ways to avoid churning in future.
•	Create a dashboard for the call centre manager about customer retention.

## Inputs
Refer 02 Churn-Dataset.xlsx
•	Customers who left within the last month.
•	Services each customer has signed up for: phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
•	Customer account information: how long as a customer, contract, payment method, paperless billing, monthly charges, total charges and number of tickets opened in the categories administrative and technical.
•	Demographic info about customers-gender, age range, and if they have partners and dependents.
•	Churn-Whether they stopped using the product or service or remained active.
1.	Yes-stopped using the service
2.	No- still a customer.
•	numAdminTickets → The number of administrative tickets a customer has opened. These could relate to billing issues, account modifications, contract changes, or other non-technical inquiries.
•	numTechTickets → The number of technical support tickets a customer has raised. These are likely related to service disruptions, troubleshooting, or other technical issues.
•	tenure → The length of time a customer has been with the company. This is usually measured in months and helps determine customer loyalty or the likelihood of churn.
•	Indicators of dissatisfaction and potential churn,
o	higher number of tickets
o	shorter tenure

## Data Visualization and Analysis using Power BI

Total calls = COUNT(Table1[Call Id])
Calls Answered = CALCULATE(COUNTROWS(Table1),Table1[Answered (Y/N)]="Y")
Calls Abandonded = CALCULATE(COUNTROWS(Table1),Table1[Answered (Y/N)]="N")
Calls Resolved = CALCULATE(COUNTROWS(Table1),Table1[Resolved]="Y")


Following are the key findings from the data analysis:

Out of the total customers, 1,869 have churned, while 5,174 remain active.
Churned customers have raised 3,058 support tickets in total.
The percentage of churned customers who raised tickets is 94.48% (1,766 out of 1,869).

Technical issues are a major concern, as 2,173 of the tickets were tech-related, compared to 885 administrative tickets.
870 churned customers (46.55%) had a tenure of less than one year.
Among churned customers, 93.95% had internet service, 90.90% had phone service, and 80% had both.

## Conclusions

Reduce Support Ticket Volume
The high ticket rate among churned customers indicates dissatisfaction. Addressing technical issues proactively and improving support efficiency may help in reducing churn.

Focus on New Customers
Since 55.55% of churned customers had a tenure of less than one year, improving the onboarding experience and providing better early-stage support could enhance customer retention.





