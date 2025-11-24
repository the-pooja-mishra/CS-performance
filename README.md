# customer support performance dashboard

## Project Overview

This project analyzes customer support efficiency and escalation trends across multiple social media channels.  
It demonstrates skills in **data generation, cleaning, analysis, and visualization** using **Python & Power BI**.

##  Objectives

1. Analyze ticket trends over time

2. Measure agent performance

3. Track SLA KPIs: response time & resolution time

4. Understand customer satisfaction through ratings

5. Provide actionable insights for Support Managers

## Tools & Technologies Used

| Phase                         | Technology            |
| ----------------------------- | --------------------- |
| Data Generation               | Python, Faker, Pandas |
| Data Cleaning & Processing    | Pandas, NumPy         |
| Data Modeling & Visualization | Power BI              |
| File Formats                  | CSV                   |

## Dataset Details

| Feature | Values |
|--------|--------|
| Total Tickets | 17,000 |
| Agents | 20 |
| Channels | 6 |
| Date Range | Last ~180 days |

### Channels Used

- Twitter  
- Escalation Email  
- LinkedIn  
- Reddit  
- Facebook  
- Instagram  

## Data Cleaning (Python)

- Handled Missing Values  
- Created Response & Resolution Time  
- Fixed “Unknown agent_id”  
- Removed incorrect timestamps 

# Power BI — Data Modeling + DAX

## Key Measures:

Total Tickets = COUNTROWS(customer_support_tickets_ready)

Resolved Tickets = CALCULATE([Total Tickets], customer_support_tickets_ready[status] = "resolved")

% Resolved Tickets = DIVIDE([Resolved Tickets], [Total Tickets])

Average Rating = AVERAGE(customer_support_tickets_ready[rating])

Avg Response Time (hrs) = AVERAGE(customer_support_tickets_ready[response_time_hrs])

Avg Resolution Time (hrs) = AVERAGE(customer_support_tickets_ready[resolution_time_hrs])


## Dashboard Features

| Visual                 | Insight                                        |
| ---------------------- | ---------------------------------------------- |
| KPIs                   | Support health: Resolution %, Avg time, Rating |
| Channel Distribution   | Where users escalate most                      |
| Issue Type Breakdown   | Product & service gaps                         |
| Agent Performance      | Efficiency & workload                          |
| Ratings                | Customer satisfaction trend                    |
| Ticket Trend Over Time | Peak escalation periods                        |

## Key Insights & Business Value

Operational Wins
- 95%+ tickets resolved → strong SLA performance
- Facebook & Twitter generate highest escalations → channel staffing needed
- Login & transaction issues” highest volume → product improvement focus

Customer Experience
- Avg rating ~4/5 → overall positive sentiment
- Low-rated tickets correlate with long resolution time → optimize workflows

Actionable Recommendations
- Support agents specializing in transaction issues
- Improve self-help for login problems
- Hire more staff during peak escalation months

https://github.com/the-pooja-mishra/CS-performance/blob/main/CSPD%20Screenshot.png

### Author
Pooja Mishra

Aspiring Data Analyst — Skilled in Python, SQL, and Power BI
 
 LinkedIn: www.linkedin.com/in/pooja-mishra-7b27191a3
