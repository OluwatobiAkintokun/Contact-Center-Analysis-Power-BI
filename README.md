# CONTACT-CENTRE-ANALYSIS

# Introduction
A Contact Center Manager is looking for transparency and insight into the data they have at the Contact Center. The manager wants an accurate overview of long term trends in customer and agent behaviour.

# Business Questions
The Contact Center manager has sought a comprehensive data analysis to address the following inquiries.

1.	Customer satisfaction rating
2.	Total calls Answered and Rejected
3.	Total calls Resolved and Unresolved
4.	Agent’s performance quadrant
5.	Average speed of answer
6.	Number of Calls by Topic
7.	Number of Calls by Month
8.	Number of Calls Answered and Rejected by Month
9.	Agent with the highest satisfaction rating
10.	Agent with the least satisfaction rating


# Dataset
The Contact center dataset consists of the following column names: Call Id,	Agent, Date, Call Time, Topic, Answered (YES/NO), Resolved (YES/NO), Speed of answer in seconds, AvgTalkDuration, and Satisfaction rating. The raw data contains 5000 rows and 10 columns.

# Data cleaning and transformation
The data cleaning and transformation were carried out using Power BI. The following actions were taken to enhance the quality and structure of the data.

- I updated the 'Resolved' column, by replacing 'Y' with 'Resolved' and 'N' with 'Unresolved'.
- I updated the 'Answered' column, by replacing 'Y' with 'Answered' and 'N' with 'Rejected'.
- To determine the total number of calls, I created a measure using DAX expression. The formular used for this is: Total Calls = COUNT('Contact Center Performance'[Answered]).
- I created a new column to calculate total number of calls answered.  The formular used for this is: Calls Answered = IF('Contact Center Performance'[Answered] ="Answered",1,0).
- I created a new column to calculate total number of calls rejected. The formular used for this is: Calls Rejected = IF('Contact Center Performance'[Answered] ="Rejected",1,0). 
- I created a new column to calculate total number of calls resolved. The formular used for this is: Call Resolved = IF('Contact Center Performance'[Resolved]="Resolved",1,0).
- I created a new column to calculate total number of calls unresolved. The formular used for this is: Calls Unresolved = IF('Contact Center Performance'[Resolved]="Unresolved",1,0).

# Data analysis, insights and recommendation

Q1. Customer satisfaction rating


Insight:


Q2. Total calls Answered and Rejected


Insight:


Q3. Total calls Resolved and Unresolved


Insight:


Q4. Agent’s performance quadrant


Insight:


Q5. Average speed of answer


Insight:


Q6. Number of Calls by Topic


Insight:


Q7. Number of Calls by Month


Insight:


Q8. Number of Calls Answered and Rejected by Month


Insight:


Q9. Agent with the highest satisfaction rating


Insight:

Q10. Agent with the least satisfaction rating


Insight:


