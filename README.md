# Cyclistic Bike Analysis


### Introduction:

In this case study, I aim to conduct data analysis for a fictional bike-share company with the objective of enhancing rider attraction. Throughout this process, I will showcase my proficiency and expertise as a junior data analyst by executing various real-world tasks. I will adhere to the fundamental steps of the data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.

### About the Company:
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system at any time. 

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends.

### Ask
#### Business Tasks
Since our team will design a new marketing strategy to convert casual riders into annual members, Lily Moreno, a marketing director, and a stakeholder in this project, wants to know the difference in the use of the Cyclistic Program between the annual members and casual riders.

### Prepare
A twelve-month dataset of Cyclistic historical trip data spanning from January 2020 to December 2020 is accessible to the public. These datasets are extensive and provided in a CSV format, organized in a zipped folder on a monthly basis. Each dataset comprises several data columns, including:

- ride_id
- rideable_type
- started_at
- ended_at
- start_station_name
- start_station_id
- end_station_name
- end_station_id
- start_lat
- start_lng
- end_lat
- end_lng
- member_casual

### Process
In this phase, I employed Power BI for ETL (Extract-Transform-Load) process utilizing Power Query mode.
#### Extract
In Power BI, I initiated the extraction process by extracting the 12 CSV files, each representing a month of Cyclistic historical trip data from January 2020 to December 2020. This initial step involved importing the data into Power BI's Power Query mode, where I could efficiently perform data cleansing, tranasforming, and loading tasks.

#### Transform
Once the data was imported, I began the transformation process by carefully examining each dataset. This involved identifying any inconsistencies, missing values, or anomalies that needed to be addressed before proceeding with the analysis. Using Power Query's robust set of transformation tools, I meticulously cleaned the data, ensuring its accuracy and integrity.

After cleaning the data, I meticulously split the "started_at" and "ended_at" columns by the delimiter to create separate Date and Time columns named "started_at.date" and "ended_at.time", respectively. This step allowed for better organization and analysis of data within the dataset.

Following the split, I further refined the Date columns by extracting the Year, Month, and Day components from both "started_at.date" and "ended_at.date". This extraction process enabled a more analysis of  trends and patterns within the data.

To enhance readability and visualization in subsequent charts, I extracted the first three characters of the Month from the "started_at.date" and "ended_at.date" columns. This transformation ensured that the Month labels were presented in a formal and abbreviated format, providing clearer interpretation of the data.

After transforming the Date columns, I proceeded to calculate the total ride length for each trip. This involved subtracting the "started_at.time" from the "ended_at.time" to determine the duration of each ride. By quantifying ride length in this manner, I obtained valuable insights into the usage patterns and behaviors of Cyclistic users, which could inform strategic decision-making for the bike-share company.

![Power Query](https://github.com/aslan0212/CyclisticBikeAnalysis/assets/140794262/54e746a8-7bec-4b13-8743-1503f9ceb210)

#### Load

After the transformation process, I "Close & Apply" to start with the visualization of charts in providing and fulfilling the business task for the project.

## Analyze and Act
In analyzing this dataset, I created a page for Insights and Recommendations that I gathered in analyzing the dataset. 

#### Home Page

![Home_Dashboard](https://github.com/aslan0212/CyclisticBikeAnalysis/assets/140794262/d36c2410-677a-4617-b2f0-0456f25f6069)

#### Stations Page

![Stations_Dashboard](https://github.com/ochengco-paolo/CyclisticBikeAnalysis/assets/140794262/9446362f-f884-4dd2-b70e-a993505e0ebd)


#### Insights Page

![Insights_Dashboard](https://github.com/aslan0212/CyclisticBikeAnalysis/assets/140794262/6743c802-6623-4181-b88f-42b9092d38b1)

