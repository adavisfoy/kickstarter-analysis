# Kickstarting with Excel
---
## Overview of Project/Project Purpose: Explain the purpose of this analysis.
I pursued this further analysis of our data set to provide Louise with insights regarding the outcomes of other Kickstarter theater campaigns based on their launch 
date and funding goals. Louise requested this analysis given that she nearly met her funding goal for her play, *Fever*, and is hoping to identify strategies that could increase 
her probability of success in future fundraising campaigns. The purpose of this analysis was to identify whether the timing of her kickstarter campaign was off or if her funding goal was unrealistic.    
## Analysis and Challenges
I first reviewed the details of Louise's kickstarter campaign for *Fever*. The funding round for *Fever* began on **6/23/2016** and ended on **7/11/2016**.
Despite the short length of her campaign (approximately 2.5 weeks), *Fever* was eighty-six percent funded and she only missed her goal by 400 dollars.   
### Analysis of Outcomes Based on Launch Date
* In order to analyze outcomes based on launch date, I created a new column called **"Years"** and utilized the **YEAR()** Excel function to convert the **"Date Created"** to a year. 
* I then created a pivot table and associated chart for **"Theater Outcomes by Launch Date."** I filtered the pivot table based on the "Parent Category" of "theater" and the new 
  "Years" field.
* **Other Pivot Table Parameters: Columns** = Outcomes; **Rows** = Date Created Conversion; **Values** = Count of outcomes
* I then created a line chart with markings for data visualization purposes, displaying the Month of the "Date Created" on the x-axis and a count of outcomes on the y-axis.
![link to image 1]
---
### Analysis of Outcomes Based on Goals
---
     - For Deliverable 2, I created a new Excel sheet to provide the basis for another line chart representing the data for the percentage of successful, failed, and canceled plays
       based on their funding goals. 
     - In the new sheet, I created the columns as outlined in the module, and utilized the COUNTIFS() formula to calculate the "Number Successful," "Number Failed," and "Number Canceled" 
       for the 12 different funding goal levels. The COUNTIFS() formula gave me the ability to calculate these numbers while filtering the data based on multiple criteria ranges and 
       criteria at the same time. The filters included: "outcome," "goal" amount, and the "Subcategory" of "plays." 
     - I utilized the SUM() formula to populate the "Total Projects" column.
     - I also utilized Excel to calculate the percentage of successful, failed, and canceled projects for each goal funding level. 
     - I then utilized this data to create another line chart displaying the "Outcomes Based on Goal" showing the relationship between the goal amount ranges (x-axis) and the 
       outcome percentages (y-axis). 
---
![link to image 2]
---
### Challenges and Difficulties Encountered
     - I had issues with the COUNTIFS() formulas for calculating the Number Successful, Failed, & Canceled plays for the "Outcomes Based on Goal" calculations. I initially forgot to include 
       a range and criteria for the Subcategory of "plays." This threw off all of my calculations. When I compared it to the graph in the module, I realized that something was off. 
       After a few minutes, I realized what I did and fixed it. My graph then matched the graph in the module. My graph was also slightly off compared to the graph in the module due to the scale
       used for the x & y axis. While this is slightly subjective, I updated the scale to match the graph in the module, and they matched.     
---
## Results: Answer the following questions in complete and coherent sentences.
---
- What are two conclusions you can draw about the Theater Outcomes based on Launch Date?
     1. There is a correlation between launch date and the probability of success, with Summer being the best season for fundraising efforts. The month with the highest number of 
	successful theater campaigns (111) was May. The month with the second highest number was June (100), followed by July (87). Based on the total # of projects for each of these 
	months, the percentages of successful campaigns in May, June & July were 67%, 65%, and 63%, respectively. Therefore, Summer appears to be the best time for a theater kickstarter 
	campaign.
     2. Conversely, there is no correlation between the launch date and the probability of failure, as the number of failed theater kickstarter campaigns remains relatively stable 
	over the months of the year.     
---
- What can you conclude about the Outcomes based on Goals?
     - Louise's fundraising goal of $2885 was a reasonable goal given that 73% of successful theater campaigns fell within the range of $1000 - $4999. The percentage of success
       decreases steadily until the goal reaches a range of $35,000 to $44,999. Interestingly, 67% of projects in this funding range succeeded in meeting their goals. We would 
       need to do additional analysis to determine the underlying factors or if they were outliers. Projects with a goal above $45,000 are very likely to fail based on this data. 
       Overall, if we follow the overall trend of successes, the probability of success decreases as the goal amount increases, which is not surprising.    

- What are some limitations of this dataset?
     - I am unsure if our sample size was adequate for making any conclusions. We would need to consider our population size, margin of error, confidence level, standard deviation, etc.
       I believe that we will be covering these topics later in the course.
     - This data set is limited specifically to Kickstarter projects. While Kickstarter is a popular way to fund such projects, it is not the only way. 
     - The kickstarter data set doesn't indicate if the fundraisers are novice or expert. I would assume that less experienced fundraisers have a higher bar to clear for success.   
     
- What are some other possible tables and/or graphs that we could create?

     - Graph to evaluate how close or how far off failed campaigns were to successfully meeting funding goals. For those that nearly met their goals, it could indicate that minor strategical 
       tweaks could get the "over the finish line." For those far off their goals, it may indicate that there is another issue with the proposed play such as lack of interest. 

     - Graph evaluating whether or not projects identified as "staff picks" had a better chance at funding success. 
       Interesting read: https://thenextweb.com/news/kickstarter-kills-staff-picks-in-favor-of-official-badges-to-avoid-confusion
       This article, dated January 11, 2016, reported that the "Staff Picks" branding was often an unofficial logo added by the campaigns themselves, rather than by Kickstarter. 
       This caused confusion, adding an artificial sense of legitamacy to some projects and probably granting an unfair advantage to projects with this branding.   
       Kickstarter replaced these badges with an official "Projects We Love" badge and directed fundraisers to remove "Staff Pick" logos. The "Projects We Love" heart logo is an 
       official, unpaid, endorsement by Kickstarter.   

