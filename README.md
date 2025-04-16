# Cardiovascular Disease Data Analysis Using Power BI

## Analysis Purpose
Cardiovascular diseases (CVD) are the leading cause of death globally, taking an estimated 17.9 millions lives every year. They are a broad group of disorders of heart and vessels, including coronary artery disease (CAD), cerebrovascular disease, peripheral artery disease (PAD), and aortic atherosclerosis. According to the studies, the risk factors for cardiovascular diseases are unhealthy diet, physical inactivity, obesity, high bloor pressure, high cholesterol, smoking and alcohol intake. Identifying those individuals at highest risk of CVDs and ensuring they receive appropriate behavior change & treatment can prevent premature deaths.

In this project, given the facts and dataset, we want to explore how the different risk factors correlate to the presence and diagnosis of CVD. What are the key influencers and how they can be addressed in priority?

## About the data source
[Kaggle dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)

This dataset contains 70000 participants' data including their gender, age and physical conditions, and whether or not they are diagnosed with CVD.

1. Age | int (days)
2. Height | int (cm) 
3. Weight | float (kg)
4. Gender | categorical code 1:women 2:men
5. Systolic blood pressure | int 
6. Diastolic blood pressure | int 
7. Cholesterol | 1: normal, 2: above normal, 3: well above normal 
8. Glucose | 1: normal, 2: above normal, 3: well above normal 
9. Smoking | binary 
10. Alcohol intake | binary
11. Physical activity | binary 
12. Presence or absence of cardiovascular disease | binary

## Development Overview
The ETL diagram is shown below. A one-time data extract was run from csv to Microsoft SQL server using SSIS. The data is transformed, analyzed and visualized in Power BI.

![alt text](https://github.com/YiningHuang15/cardiovascular_disease_data_analysis/blob/main/viz/etl_diagram.png)

![alt text](https://github.com/YiningHuang15/cardiovascular_disease_data_analysis/blob/main/viz/pbi_cvd_dashboard.png)

According to the analysis, it is found that high bloor pressure, high cholesterol and obesity are key influencers for CVD among these participants and need to be taken care in priority.

## Folder Structure
- dat: csv
- pbix: Power BI Workbook
