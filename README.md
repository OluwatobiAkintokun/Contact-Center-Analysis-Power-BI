# CONTACT-CENTRE-ANALYSIS

# Introduction
A Contact Center Manager is looking for transparency and insight into the data they have at the Contact Center. The manager wants an accurate overview of long term trends in customer and agent behaviour.

# Business Questions
The Contact Center manager has sought a comprehensive data analysis to address the following inquiries.

1.	Customer satisfaction rating
2.	Total calls Answered and Abandoned
3.	Total calls Resolved and Unresolved
4.	Agent’s performance statistics
5.	Average speed of answer
6.	Number of Calls by Topic
7.	Number of Calls Answered and Abandoned by Month
8.	Number of Calls Resolved and Unresolved by Month
9.	Agent with the highest satisfaction rating
10.	Agent with the least satisfaction rating


# Dataset
The Contact center dataset consists of the following column names: Call Id,	Agent, Date, Call Time, Topic, Answered (YES/NO), Resolved (YES/NO), Speed of answer in seconds, AvgTalkDuration, and Satisfaction rating. The raw data contains 5000 rows and 10 columns.

# Data cleaning and transformation
The data cleaning and transformation were carried out using Power BI. The following actions were taken to enhance the quality and structure of the data.

- I updated the 'Resolved' column, by replacing 'Y' with 'Resolved' and 'N' with 'Unresolved'.
- I updated the 'Answered' column, by replacing 'Y' with 'Answered' and 'N' with 'Not Answered'.
- I renamed the sheet from Sheet1 to ‘Contact Center Performance’.
- I changed the data type for ‘Time’ and ‘AvgTalkDuration’ columns to a time data type.
- I created a measure using DAX to determine the total number of calls. The formular used for this is: Total Calls = COUNT('Contact Center Performance'[Answered]).
- I created a new column to calculate total number of calls answered.  The formular used for this is: Calls Answered = IF('Contact Center Performance'[Answered] ="Answered",1,0).
- I created a new column to calculate total number of calls abandoned. The formular used for this is: Calls Abandoned = IF('Contact Center Performance'[Answered] ="Not Answered",1,0). 
- I created a new column to calculate total number of calls resolved. The formular used for this is: Call Resolved = IF('Contact Center Performance'[Resolved]="Resolved",1,0).
- I created a new column to calculate total number of calls unresolved. The formular used for this is: Calls Unresolved = IF('Contact Center Performance'[Resolved]="Unresolved",1,0).

# Data analysis, insights and recommendation

Q1. Customer satisfaction rating

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/d4e5c519-c70f-41ff-9fe2-c84cc6ff52b3)


Insight: Based on this analysis, the overall customer satisfaction rating of 3.40 suggests that there is room for improvement in customer satisfaction. My recommendations for the Contact Center Manager are listed below.
- Identify specific areas in the customer journey where satisfaction is lower. This could include issues with wait times, agent responsiveness, or the resolution process. Figuring out where things are going wrong can guide the business in making fixes that address those exact issues.
- Compare the current satisfaction rating with industry benchmarks or competitors. Understanding how your contact center performs relative to others in the industry can provide context and highlight areas for improvement. 
- Create more communication channels such as live chat, email and web support. This helps the customers to access support easily through their preferred channels and receive timely and helpful responses.
- The business should provide specific, concrete and practical suggestions for enhancing customer satisfaction. These could include process improvements, training programs for agents, technology upgrades, or changes in customer engagement strategies.

# 

Q2. Total calls Answered and Abandoned

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/f92d141b-b5c0-42ef-813a-2506e69228e1)


Insight: My analysis reveals that 81% of calls that came in were answered while 19% of calls were abandoned. Balancing the call answering and abandoned rates is crucial for achieving a positive impact on customer satisfaction. Aiming for a high percentage of answered calls, such as 95% or higher, is generally a positive goal. This ensures that customers can easily reach a representative. A call abandoned rate of 5% or lower is often considered acceptable. Abandoned calls represent missed opportunities to address customer needs, resolve issues, or potentially make sales. This could contribute to a negative brand image, affecting customer trust and loyalty. My recommendations for the Contact Center Manager are listed below.
- Evaluate the current staffing levels and consider adjusting them to better align with the call volume. If a significant number of calls are being abandoned, it may indicate that the contact center is understaffed during peak times.
- Consider implementing a call back option for customers who cannot be immediately accommodated. This can help manage high call volumes without compromising customer satisfaction, as customers are given the choice to be contacted when an agent is available.
- Invest in self-service options such as interactive voice response (IVR) systems, comprehensive FAQs, or online knowledge bases. This can empower customers to find answers to common queries without the need for a live agent, reducing the overall call volume.

# 

Q3. Total calls Resolved and Unresolved

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/1d954e0f-842a-44cd-8c35-acd650121d71)


Insight: Based on this analysis, 72.92% of customer's issues were resolved, while 27.08% were unresolved. A target resolution rate of 95% or higher is often considered good practice. The goal is to ensure that many customer issues are effectively resolved during the initial interaction, minimizing the need for follow-up contacts. Resolving customer issues promptly is crucial for customer retention. High unresolved rates may lead to customer churn, as dissatisfied customers may seek alternatives. Prioritizing issue resolution not only distinguishes businesses in the market but also contributes to attracting and retaining customers. To ensure that calls are resolved as quickly as possible in a contact center, here are my recommendations for the Contact Center Manager:
- Use real-time analytics to regularly track key performance metrics, such as call volume, agent availability, and resolution times. This helps to analyse the reasons for unresolved calls, and also to implement strategies for improvement. This could involve additional training for agents, process improvements, or enhancements to self-service options. 
- Invest in advanced call routing systems that direct calls to the most appropriate department. Efficient routing ensures that customers are connected to the right team quickly, minimizing transfer times and resolution delays.
- Implement knowledge management systems that empower agents to quickly access relevant information and solutions. A centralized repository of FAQs, troubleshooting guides, knowledge hub, and best practices can quicken issue resolution and reduce the need for lengthy research.

# 

Q4. Agent’s performance statistics

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/82b157e9-5f07-405c-9c1f-7f933a99e8d0)



Insight: Agent Performance Statistics refer to the quantitative metrics used to assess the individual performance of contact center agents. These statistics provide valuable insights into how well agents are performing their duties and contributing to the overall success of the contact center. The Agent Performance Statistics table above shows the total calls, calls answered, calls abandoned, calls resolved, calls unresolved, satisfaction rating, avg speed of answer and call durations of each agent. These performance statistics is essential for the contact center manager to identify strengths and weaknesses in agent performance. This will enable the business to allocate resources effectively, and implement targeted training and improvement initiatives. Regularly analyzing these metrics enables data-driven decision-making and contributes to the overall success of the contact center in delivering exceptional customer service.

# 

Q5. Average speed of answer

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/3bd3b023-68f1-45e9-b54a-ae9da38be02f)


Insight: The Average Speed of Answer derived from this analysis is 67.22. Average Speed of Answer (ASA) is a key performance metric in a contact center, measuring the average time it takes for incoming calls to be answered by a live agent. ASA is a crucial indicator of how quickly customers can connect with a representative and is a significant factor in overall customer satisfaction. This is typically measured in seconds. The lower the Average Speed of Answer, the better, as it indicates that calls are being answered promptly. A low Average Speed of Answer contributes to a positive customer experience by minimizing the time customers spend in the queue and demonstrating responsiveness on the part of the contact center. To improve the Average Speed of Answer (ASA) for agents in contact center, consider the following recommendations:
- Cross-train agents to handle a variety of inquiries and tasks. This increases flexibility in workforce management, allowing agents to assist in different areas during peak times, thereby reducing the overall wait time for customers. 
- Use historical data and forecasting tools to better predict call volumes during peak hours. 
- Adjust staffing levels accordingly to ensure that an adequate number of agents are available to handle incoming calls promptly.

# 

Q6. Number of Calls by Topic

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/25a4394c-9ea6-4e78-998c-9d4d73bc8202)

Insight:


Q7. Number of Calls Answered and Abandoned by Month


![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/7510d577-c239-4477-a758-9e89319b615b)


# 

Q8. Number of Calls Resolved and Unresolved by Month

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/496ac534-bec5-49bc-858f-d1a6371ef575)

# 

Q9. Agent with the highest satisfaction rating


![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/b65d8e81-0bf6-42e8-ae48-977703621152)


Insight:

# 

Q10. Agent with the least satisfaction rating

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/5180e1b7-2241-413c-8d76-6372b1a9ffd7)


Insight:


# Dashboard
I created a user-friendly and interactive dashboard with Power BI to showcase the outcomes of the data analysis.

![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/d2176255-585a-4906-b439-659af982674f)


![image](https://github.com/OluwatobiAkintokun/CONTACT-CENTRE-ANALYSIS/assets/137109080/292dcb01-3c52-4345-b7f4-72e0d41675eb)


Dataset from theforage.com (Accessed: July 2023)
