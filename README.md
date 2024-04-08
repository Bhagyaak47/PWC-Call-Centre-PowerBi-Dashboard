# PWC-Call-Centre-PowerBi-Dashboard

PwC Power BI Virtual Case Experience Task 1- Call Centre Analysis and Dashboard

Problem Statement :
In this Project,I have created a dashboard in Power Bi for the call centre manager that reflects all relevant Key Performance Indicators(KPI's) and matrics in the dataset.

Possible KPI's & their DAX formulas :
1.Total Calls = COUNT(Sheet1[Call Id])
2.Answered = CALCULATE([Total Calls],Sheet1[Answered (Y/N)]= "Y")
3.Not Answered = CALCULATE([Total Calls],Sheet1[Answered (Y/N)] ="N") 4.Resolved = CALCULATE([Total Calls],Sheet1[Resolved]= "Y")
5.Unresolved = CALCULATE([Total Calls],Sheet1[Resolved]= "N")
6.Answered % = DIVIDE('All measures'[Answered],[Total Calls]) 7.Not Answered % = DIVIDE([Not Answered],[Total Calls])
8.Resolved % = DIVIDE('All measures'[Resolved],[Total Calls]) 9.Unresolved % = DIVIDE([Unresolved],[Total Calls])

Dataset:
The dataset used for this task was presented by https://www.theforage.com

Data Cleaning/ Preparation:
1.The data consists of over 5000 rows and 16 columns 2.Changed the datatypes of certain columns
3.The month name and weekday are extracted for further analysis.
4.Replaced Y/N with Yes/No for better readability.
5.Sorted the month and week in charts using the daynum and monthnum columns. 6.Various Dax Measures were created beforehand like Average satisfaction rating, average speed of answers in minutes/seconds, Total calls etc.

Questions to be Answered :
1.Important Overall metrics like : i. Total Calls ii. Average Speed of Answer in mins iii. Average talk duration in mins iv. Average Satisfaction rating and target rating
2.Agent statistics like totals calls, total resolved calls, answered calls, satisfaction ratings etc
3.What was each month's stat ie calls answered- Yes and no?
4.What was the total number of calls answered and resolved?
5.What day of the week receives the most calls? 6.What was the Topic of Answered and Not Answered calls? 7.Which Agent Resolved the most issue & Which agent not answered most of the calls ?
![CALL CENTRE_001](https://github.com/Bhagyaak47/PWC-Call-Centre-PowerBi-Dashboard/assets/152842490/2f6a786a-90c6-4c49-9c02-a2f82cc904bd)
![CALL CENTRE_002](https://github.com/Bhagyaak47/PWC-Call-Centre-PowerBi-Dashboard/assets/152842490/03ad7808-34d3-44cc-b512-192c227e96ac)


Insights :
1.The dashboard is filtered by various columns like date,agents, months and calls by topic 2.The total calls made in the 3 months are 5000 and the average satisfaction rating is around 3.40 whereas it should be around 4.5 for most customer satisfaction.
3.Out of all three months, January received the most calls(1772) and around 1455 were answered and 317 were not answered. That was most probably because January month had the highest number of issues which were resolved (1311 issues resolved) and which can be seen because February and March had fewer calls.
4.Out of the total calls only 72.92% are resolved over the three months and 27.08% remain unsolved.
5.Streaming and technical support were the topics for which the most calls were received followed by payment-related issues.
6.Monday and Saturday were the days where most calls were recorded followed by Sunday. 7.Becky has the quickest average speed of answer (65.33sec) whereas Joe is the agent who answers late(70.99sec) because of which the average satisfaction rating of Joe is the lowest (3.33) and Martha has the highest satisfaction rating(3.47).
8.Jim received the highest number of calls where he answered 536 of calls and resolved 485 of calls.

Recommendations:
1.The decreasing customer satisfaction rating should be analysed because compared to the January performance both months received almost the same performance but then why the satisfaction rating decreased? Were the issues not resolved properly?
2.The average speed of the answer should be decreased because 70.99sec to answer is on the higher side
3.The streaming and technical aspects of the business should be analysed properly because they received the highest number of calls. 4.Certain benefits/incentives can be provided to employees who get the highest satisfaction rating or depending on other factors like most reloved or most answered every month .
6.The resolve rate should be increased which will lead to a higher satisfaction rate eventually.
