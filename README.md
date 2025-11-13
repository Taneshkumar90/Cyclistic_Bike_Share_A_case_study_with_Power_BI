# Cyclistic's bike share - case-study-with-power-BI

## INTRODUCTION
- This capstone project is belong to Google Data Analytics Professional Certificate Course. In this case study, I will be analyzing a public dataset for a fictional company called Cyclistic, provided by the course. Here, I will be using Power BI Tool for this analysis because of its potential benefits to reproducibility, transparency, easy statistical analysis tools and data visualizations.

  ![image](https://github.com/user-attachments/assets/39335853-f77e-4bef-afca-8f2edd1b1d37)

- ## The following sets of data analysis process will be followed:

    -    Ask
         

    -   Prepare
         
    -   Process

    -  Analyze

    -   Share

     -  Act
### **Scenerio**

You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members.But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data.

## ASK

- Three questions will guide the future marketing program:
   - 1. How do annual members and casual riders use Cyclistic bikes differently?

   -  2. Why would casual riders buy Cyclistic annual memberships?

   - 3. How can Cyclistic use digital media to influence casual riders to become members?

Lily Moreno (director of marketing and my manager) has assigned me the first question to answer: How do annual members and casual riders use Cyclistic bikes differently?

### Key tasks

- 1: Identify the business task
   - The main business obejective is to design marketing strategies aimed at converting casual riders into annual members by understanding how they differ.
     
- 2: Consider key stakeholders
   - The key stakeholders are the Director of Marketing (Lily Moreno), Marketing Analytics team, and Executive team.
 
### Deliverable

- 1: A clear statement of the business task
   - To find the differences between the casual riders and annual members

## PREPARE

- I will use Cyclistic’s historical trip data to analyze and identify trends.The data has been made available by Motivate International Inc. under this [license](https://divvybikes.com/data-license-agreement). Datasets are available here [link](https://divvy-tripdata.s3.amazonaws.com/index.html).
### Key tasks

   - 1: Download data and store it appropriately.
       - Data has been downloaded and copies have been stored securely on my computer.
   - 2: Identify how it’s organized.
       - The data is in CSV (comma-separated values) format, and there are a total of 13 columns.
   - 3: Sort and filter the data.
      - For this analysis, I will be using data for the year 2019 and 2020.
   - 4: Determine the credibility of the data.
       - For the purposes of this case study, the datasets are appropriate and will enable me to answer the business questions. The data has been made available by Motivate International Inc. This is public data that I can use to explore how different customer types are using Cyclistic bikes. But data-privacy issues will prohibit me from using rider’s personally identifiable information and this will prevent me from determining if riders have purchased multiple single passes. All ride ids are unique.

### Deliverable

- 1: A description of all data sources used
   - The main source of all the data used was provided by the [Cyclistic Company](https://divvy-tripdata.s3.amazonaws.com/index.html).
   - Download and save all Data in a folder
   - Import all data to Power BI
   - Load and merg all 13 tables into a single file
      - I made sure all the data sets have the same number of columns and also the name of each columns are the same before merging it all together
    
## PROCESS
- **Cleaning up data and adding data to prepare for analysis**

### Key tasks

- 1: Check the data for errors.

- 2: Choose your tools.

- 3: Transform the data so you can work with it effectively.

- 4: Document the cleaning process.

### Deliverables

- 1: Documentation of any cleaning or manipulation of data.
  - I inspected the new table that has been created by the following steps
    - 1: Open your **Transform data** page and create a column which is named ride_length.Calculate the length of each ride by subtracting the column started_at from the column ended_at (for
 example, =[ended_at]-[started_at]) and format as **duration**  deleted all negative or zero duration rows.
    - 2:  Create a column called day_of_week, and calculate the day of the week that each ride
 started using the WEEKDAY command(for example, WEEKDAY([started_at])).
 Format as text.
- 2: Deleted all duplicate data by selected all.
- 3:  Proceed to the analyze step.

## ANALYZE

All the data have been strored appropriately and has been prepared for analysis, so they are ready for exploration.
### Key tasks

- Aggregated data to make it useful and accessible.
- Organize and format data.
- Perform calculations.
- Identify trends and relationships.
### Deliverables

#### A summary of My analysis:

### Visualise the **distribution of casual riders and member rider** by  PIE-CHART

<p align="center">
  <img src="https://github.com/Taneshkumar90/Cyclistic_Bike_Share_A_case_study_with_Power_BI/blob/2d26fc86a6c9422a6cebff537df92c6b3e3eb65c/Screenshot%202025-11-11%20214450.png" alt="HR Dashboard" width="1000">
</p>


- From the above graph, we can observe that there are more no. of member(annualy) riders compared to casual riders.
- Though casual members are less but they ride more time than member(annual)

### Visualise the **distribution of number of rides b/w casual riders and member riders** by line chart




<img width="1214" height="699" alt="WEEKLY_NO _OF_RIDERS" src="https://github.com/user-attachments/assets/fdcb0ad1-4eab-4b3d-a6d0-d402087baf96" />



- Here we can see on **saturday** casual riders are on peak and on thursday and wednesday member riders are on peak. 
- We also can observe that duration of casual riders very high camprison to members riders on the contrary numbers of member riders is more.

### Visualise the **number of rides b/w casual riders and member rider** on the basis of  different bike types by pie-chart

<img width="1210" height="701" alt="BIKE_SHARE" src="https://github.com/user-attachments/assets/1f299d60-1a42-427b-80c2-7da808f3583c" />

 

- From given charts we can see that docked bike is  used only by casual member
- Number of rides on docked bikes is least comparison to others
- Annual members mostly uses **Classical** and **Electrical** bikes
- The electricsl bikes are the most favored option among users.


### Visualise the **distribution of ride duration b/w casual riders and member rider** by line chart

  
  


<img width="1213" height="702" alt="RIDE_LENGTH_DISTRIBUTION" src="https://github.com/user-attachments/assets/594b3b9a-6577-4723-a445-76c46ee6428e" />


- Here we can see on **saturday** casual riders are on peak in  spending time. 
- On thursday and wednesday member riders are on peak in spending time.
- We also can observe that when member riders duration increase and simultanously casual riders duration decrease and vice-versa.

### Visualise the **distribution of riders** in diffrent areas of chicago 




<img width="1214" height="697" alt="RIDERS&#39;_MAP" src="https://github.com/user-attachments/assets/6773c0c6-c14c-4a2b-a892-372436f2623c" />

- From above map number of casaul riders more on coastal areas of chicago
- As distance increases from coastal areas number of Member riders increases to comparison to casual riders almost tends to 100%.
  
### Visualise the **distribution of riders** in diffrent started_stations in  chicago 





<img width="1211" height="701" alt="TOP_STATIONS" src="https://github.com/user-attachments/assets/77736507-e927-4e99-ae5e-bc2978d98dc3" />

- There are many top stations where number of casual members are much more.
-  Streeter Dr & Grand Ave, DuSable Lake Shore Dr & Monroe St are top stations where casual members are more comparison to member riders

### Visualise the **average distribution of ride length(duration) in riders** 




<img width="1279" height="240" alt="AVG_RIDE_LENGTH" src="https://github.com/user-attachments/assets/515e5ef8-6103-4ae5-83c8-74b04e46265c" />


- Its clear casual riders spend  almost  time on bike to ride. 


## SHARE

**This phase involves using visualization to share my findings and can be done by presentation**.

### Key tasks

- 1: Determine the best way to share your findings.

- 2: Create effective data visualizations.

- 3: Present your findings.

- 4: Ensure your work is accessible.

### Deliverables

Supporting visualizations and key findings


Your top 3 recommendations based on your analysis

## ACT

This phase will be carried out by the executive team, Director of Marketing (Lily Moreno) and the Marketing Analytics team based on my analysis.

### Conclusion

- 1: Members have more bikes compared to casual riders.

- 2: We have more members riding in all months compared to casual riders.

- 3: Casual riders travel for a longer time period.
- 4: Since Members ride more throughout the entire weekday while the casual riders also have a high ride record during the weekends(Saturday and Sunday) compared to the other days of the week.


### Deliverable

- Our top 3 recommendations based on your analysis

   - 1: Since casual riders are  more popular on the weekends, we can consider having a weekend membership option.
   - 2: We can take the Top 20 starting stations and if a casual rider leaves from it, send them an ad for membership. We also market to casual riders who finish at the Top 20 ending stations.
   - 3: Host fun biking competitions with prizes at intervals for casual riders on the weekends. Since there are lot of members on weekends, this will also attract them to get a membership.
 
### Thank you for giving your valuable time to my project.
