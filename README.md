# SD-Padres-Payroll-Analysis

San Diego Padres Payroll Analysis 







Analytics Programming
MSBA 502 
Kymberly Patino and Oriana Caro

Project Overview and Research Question
This project examines the relationship between player salaries and on-field performance for the San Diego Padres from 2021 through 2025.
Our main research question is:
How does player salary relate to on-field performance for the San Diego Padres, and which players provide the most value for the money they are paid?
Our goal was to use Python and baseball statistics to identify patterns in player spending and provide recommendations for future payroll decisions.
Data Collection
For this project, we studied San Diego Padres player salaries and performance from 2021 to 2025. Our main data source was FanGraphs, a website that provides information about baseball player salaries, contracts, and performance statistics.
We focused on two main variables: yearly player salary and Wins Above Replacement (WAR). Salary shows the amount listed for a player in a particular season, while WAR estimates how much a player contributes compared with a replacement-level player.
We collected three types of datasets:
Payroll data: Player names, yearly salaries, and contract information.
Batting data: Performance statistics for hitters, who try to hit the baseball and help their team score.
Pitching data: Performance statistics for pitchers, who throw the baseball and try to stop the other team from scoring.
We collected five years of each dataset, giving us 15 original files.
The information included player names, seasons, yearly salaries, WAR, player positions, and contract information when available.
We used yearly payroll salary rather than Average Annual Value (AAV), which is the average amount of a contract per year. This allowed us to compare a player's listed salary with their performance during the same season.
Data Cleaning
We used Python and the pandas library to clean and organize our datasets.
First, we imported the payroll, batting, and pitching files for each season from 2021 through 2025.
Next, we checked for missing information, organized salary values into a consistent numerical format, and combined overlapping player records.
We matched player performance statistics with salary information using FanGraphs player identification numbers and the season. This helped us avoid incorrectly matching players who had similar names.
Our original batting and pitching datasets contained 414 statistical records. After cleaning and matching the data with available salary information, our final analysis included 151 matched observations: 68 hitter records and 83 pitcher records.
Some records could not be matched reliably with salary information, so they were not included in the final salary and WAR analysis.
A player-season means one player during one particular year.
We also considered that players who changed teams during a season might have salary amounts that did not exactly reflect what the Padres paid.
The final matched dataset was used for our statistical analysis.





Data Analysis
We used Python to examine whether players with higher salaries generally produce higher WAR.
First, we calculated basic statistics, including average salary, average WAR, and the highest and lowest values. This helped us understand how the Padres distribute their payroll.
Next, we used correlation analysis to measure the relationship between salary and WAR. We also used linear regression to see how well salary explains differences in player performance.
We created graphs to make the results easier to understand. These include a scatterplot comparing salary and WAR, charts showing player performance, and outputs comparing payroll spending across seasons.
We also calculated cost per WAR for players with positive WAR. This helped us compare how much the Padres spend for each unit of player performance. We excluded players with zero or negative WAR from the salary-per-WAR calculation because dividing by zero is not possible and negative WAR requires a different interpretation.
Results and Findings
Our initial research shows that the Padres have players with very different salary levels. For example, the 2025 payroll records list Xander Bogaerts at approximately $25.45 million, Fernando Tatis Jr. at $20.71 million, and Manny Machado at $17.09 million.
These differences show why it is useful to compare salaries with performance rather than looking at salaries alone.
After cleaning and combining our datasets, we analyzed 151 player-season records from 2021 through 2025. These records included both hitters and pitchers who had matching salary and performance information.
Our overall correlation between player salary and WAR was approximately 0.51. This shows a moderate positive relationship, meaning players with higher salaries generally tended to perform better.
Our R-squared value was approximately 0.26. This means salary explained about 26% of the differences in player performance in our analysis. The remaining differences may be related to factors such as injuries, age, experience, and player position.
When we looked at hitters and pitchers separately, we found:
Hitters: 68 matched records, with a correlation of 0.545.
Pitchers: 83 matched records, with a correlation of 0.43.
These findings suggest that salary and performance are related, but paying a player more does not guarantee better results.
We also calculated salary per WAR to compare how much the Padres paid for each unit of player performance. This helped us identify examples of players who provided strong value relative to their salaries.
Additional Statistical Results
The average player salary in our matched dataset was approximately $6.48 million, and the average WAR was 1.31.
Our linear regression showed a slope of approximately 0.116. This means that, in our model, an additional $1 million in annual salary was associated with approximately 0.116 additional WAR.

These findings suggest that salary is related to player performance, but it does not explain every difference between players.


Best Player Value
We also identified players who provided strong performance relative to their salaries.
In 2024, Jackson Merrill earned approximately $740,000 and produced 5.36 WAR, giving him a cost of approximately $138,000 per WAR.
In 2021, Jake Cronenworth earned approximately $585,000 and produced 3.76 WAR, giving him a cost of approximately $155,000 per WAR.
In 2024, Jurickson Profar earned approximately $1 million and produced 4.36 WAR, giving him a cost of approximately $230,000 per WAR.
These examples show that some lower-paid players can provide strong value. However, salaries can also depend on a player's experience and contract rules, so lower cost per WAR does not always mean a player has a better contract overall.


Business Recommendations
Based on our analysis, we recommend that the San Diego Padres consider both player performance and salary when making spending decisions. Our results show that higher salaries are generally related to better performance, but paying more does not always guarantee better results.
Short-Term Recommendations
In the short term, the Padres should focus on getting the most value from their current players. The team should review existing contracts and identify positions that need improvement, especially areas where additional hitting or pitching support may be needed.
Before signing new players, the Padres should compare their salaries, past performance, and injury history. This could help the team avoid spending too much money on players who may not provide enough value.
Long-Term Recommendations
For long-term planning, we used a hypothetical annual payroll budget of $220 million. This amount is an example for our project and does not represent the Padres' actual available budget.
The team should first account for money already committed to existing player contracts. Then, it can decide how much money remains for future signings, younger players, and other team needs.
We also recommend investing in player development, which means helping younger players improve their skills. This could allow the Padres to develop strong players without always relying on expensive contracts.
Overall, our recommendation is to balance short-term performance with long-term financial planning. By considering both salary and WAR, the Padres can make more informed decisions about how to spend their money.

Limitations
Our project has several limitations. First, we were only able to match 151 player-season records with salary information. This means our analysis does not include every Padres player from 2021 through 2025. Second, the salaries listed in the payroll datasets may not always equal the exact amount the Padres paid, especially when players were traded between teams. Third, our analysis focused mainly on salary and WAR. Other factors, such as injuries, age, experience, and contract length, may also affect player performance. Finally, correlation does not prove causation. 
Our results show that salary and WAR are related, but they do not prove that paying a player more money causes them to perform better. Because of these limitations, our findings should be used as one part of the team's decision-making process rather than the only factor when choosing players.
Future Improvements
In a future project, we could improve our analysis by including more information about each player, such as age, injury history, contract length, and playing time. We could also compare the Padres with other Major League Baseball teams to see whether their spending is more or less efficient. Another improvement would be to create a model that predicts future player performance based on past statistics. 
For MSBA 503, we could use these predictions to explore how the Padres might distribute a limited payroll budget across different positions. These improvements would help us move from explaining past performance to making more useful predictions about future spending decisions.
Project Files
Our GitHub repository contains the following files and folders:
README.md: The project report and instructions for running the analysis.
Data files: Original FanGraphs payroll, batting, and pitching datasets.
Jupyter Notebook (SDPadresProject.ipynb): Contains the Python code used to clean, combine, and analyze the data.
Cleaned dataset: The matched player salary and WAR information.
Results: Statistical summaries and graphs.
Presentation: Slides summarizing our findings and recommendations.





User Manual: How to Run Our Project
This section explains how to download our San Diego Padres project and repeat the analysis using JupyterLab.
Step 1: Download the Project
Open our GitHub repository.
Click Code → Download ZIP.
Extract the ZIP file onto your computer.
Open the downloaded project folder.
Step 2: Check the Project Files
The project should contain:
SDPadresProject.ipynb — Our Jupyter Notebook containing the Python analysis.
Five Padres payroll Excel files for 2021–2025.
Ten FanGraphs CSV files containing batting and pitching statistics for 2021–2025.
README.md — Our project report and user manual.
Any included charts, cleaned datasets, and presentation files.
Keep the Jupyter Notebook and the 15 original datasets in the same folder.
Step 3: Open JupyterLab
Install Anaconda from https://www.anaconda.com/download if needed.
Open Anaconda and launch JupyterLab.
In JupyterLab, navigate to the downloaded project folder and double-click SDPadresProject.ipynb.
Step 4: Install the Required Libraries
Our notebook uses pandas, matplotlib, seaborn, scikit-learn, and openpyxl.
If these libraries are not installed, open a terminal and run:
python -m pip install pandas matplotlib seaborn scikit-learn openpyxl
These libraries allow Python to read datasets, calculate statistics, run regression analysis, and create graphs.
Step 5: Run the Analysis
Make sure all 15 original FanGraphs datasets are in the same folder as the notebook.
Open SDPadresProject.ipynb in JupyterLab.
Click Run → Run All Cells.
Wait for the analysis to finish.
Review the tables, statistical results, and graphs.
Step 6: Find the Results
The notebook creates several output files, including:
Padres_Combined_WAR_2021_2025.csv — Combined player performance records.
Padres_Final_Dataset_2021_2025.csv — Player salary and WAR information.
Padres_Yearly_Summary.csv — Yearly summary statistics.
Padres_Player_Value_2021_2025.csv — Player value calculations.
Padres_Hitters_vs_Pitchers.csv — Comparison of hitters and pitchers.
Padres_Salary_vs_WAR.png — Salary versus WAR graph.
Padres_220M_Budget.png — Hypothetical budget visualization.
Step 7: Understand the Findings
Our notebook reported the following results:
151 matched player-season records.
Overall salary and WAR correlation: 0.506.
R-squared: 0.256.
Hitters' correlation: 0.545.
Pitchers' correlation: 0.426.
The results show a moderate positive relationship between player salaries and performance.
However, a higher salary does not guarantee better performance. Our findings should be considered alongside injuries, experience, contract details, and other team needs.
Data Sources and References
Our main data source was FanGraphs (https://www.fangraphs.com/)
We collected San Diego Padres payroll, batting, and pitching data for the 2021, 2022, 2023, 2024, and 2025 seasons. 
We used these datasets for educational analysis as part of our MSBA 502 Analytics Programming project and did a formal presentation in front of our cohort and professor. 
