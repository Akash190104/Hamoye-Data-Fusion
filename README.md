# Hamoye-Data-Fusion
This is the repository for the team "Data Fusion" of Hamoye Data Science Fall Internship 2023. All of our work, along with datasets, code, visualizations, and documentation will be presented in this repository. The contribution of each member could be seen as they push and commit their hard work here.

# The team:

The Table below consists of the list of all the team members in our team along with their track.

| Name | Track |
| --- | --- |
| Akash Kundu | Data Science |
| Ikenna Ajere | Data Science |
| Amir Adams | Data Science |
| Maria Ajose | Data Science |
| Chinaza Blessing Oroke | Data Science |
| Mujeeb Sunmola | Data Science |
| Oluwafemi Abiona | Data Engineering |
| Eke Mong Eke | Data Storytelling |
| Linda Owolabi | Data Storytelling |
| John Fakile | DevOps |




The team representatives are:

- Akash Kundu (Project Lead)
- John Fakile (Assistant Project Lead)
- Eke Mong Eke (Query Analyst)

# HAMOYE HDSC FALL ’23 – PREMIERE ROJECT

## Topic: Predicting Scale of Conflicts: National vs International

### Analysis of Conflicts in Africa (1997 – 2020)
~Team ***DataFusion***

### Introduction

### Problem Statement

The African continent has witnessed numerous conflicts over the years, which have had devastating effects on the lives of its citizens and the economy. Understanding the scale of these conflicts is crucial in developing effective strategies to mitigate them and prevent their escalation to an international level. This project aims to develop a machine learning model to predict the scale of conflicts in Africa as either national or international, based on available features. This project has the potential to provide valuable insights into the causes and prevention of conflicts in Africa, leading to improved conflict resolution and peacebuilding efforts on the continent.

### Aim and Objectives

The objectives of this project are to:

1.  Develop a machine learning model to predict whether a conflict is of national or international scale based on the available features.
    
2.  Identify the key features that contribute significantly to the prediction of conflict scale.
    
3.  Investigate the factors that differentiate conflicts of national scale from those of international scale, providing insights into the reasons for conflicts becoming of international importance.
    
4.  Evaluate the performance of the machine learning model using appropriate evaluation metrics and techniques.
    
5.  Explore potential strategies and recommendations for stakeholders to mitigate conflicts and prevent their escalation to an international scale.
    

Flow Process

The steps taken are illustrated with the ﬂowchart below:![](https://lh7-us.googleusercontent.com/H5MTrQYGPfkjFv8F4MziMFWl7fi5aXVjodiro4pC-8ZHho-QbuvhixkFU_2RE2WUNGBpEu_P7Xq3cTeEtOvY8u1MoshNuoaHjA8SmJq_tmol5R2rjVx0l291H4D2UeJW9WOqh3CiJZI0viSFPcIMYF1VFO2vT4E)

  

### Data Gathering:

The dataset was obtained from Kaggle via this [link](https://www.kaggle.com/datasets/lumierebatalong/africa-conflict-19972020) 

This analysis focuses on the African Conflict Dataset from 1997 to 2020. The dataset contains information for 65,535 individual observations, with each having 29 different variables associated with it.

### Data Preparation:

The following procedures were used to prepare the data:

-   **Data collection** : The dataset contains information on various variables such as event ID, event date, event type, actors involved, location, latitude, longitude, and fatalities. The dataset has missing values in some columns, such as actor2, admin3, associated actors and event notes.
    
-   **Data transformation**: The dates in the data were converted to datetime, and the latitude and longitude columns were converted to float.
    
-   **Data visualization**: Here, information was displayed using bar charts, box plots, pie charts, heatmaps, and other visual aids to facilitate clear and simple interpretation.
    

### Exploratory Data Analysis

We conducted exploratory data analysis to gain a deeper understanding of the gathered data, to provide a more comprehensive view of the data, and to identify and understand patterns that could help explain unexpected results.

As a result of this analysis, several insights were generated.

1.  The event types, battles (28.8%) and violence against civilians (28.6%) contributed the most to fatalities, which indicates the prevalence of armed conflicts and human rights abuses. Protests and riots (over 30%) also appear to be relatively common, highlighting the presence of social and political unrest.
    

![A close-up of a pie chart

Description automatically generated](https://lh7-us.googleusercontent.com/D5f7vwG0UcJ7D7pN5mL56vwMhVOl75neynlS8br92L7bhD1DwnbDfH-iETcElVHJDMg0QDgywWmga8o2ZU0P3nulLV2quezCD8H8Zx62LL0bmx6ttPIKow6pdF8kcFDsJszNQIyviLNKMBtlZnx2b1bbiixByro)

2.  We observed that in 2020, there were 10,413 reported events, making it the year with the highest count. This suggests that 2020 was a year that experienced a significant number of incidents. While between 2016 - 2019 had a significant number of reported events. It can be said that these years signify periods of heightened conflict or incidents that received substantial attention and reporting.
    

![Distribution of Event types by Year](https://lh7-us.googleusercontent.com/O0G--T1kYE_SgyM5X99M3faBKI0GfkhebOSjKBPxRsfoIXnCznt_xztdaH3i2J6sjxP5oHm9O6qZnuaa01hKub4rlKClKzjxCbijAs3_fXdMU6Vf5OmxSo7fpzYCRtqaWXKKnm6xyDSx_WZSlrUuJbilUsthbTE)

3.  The dataset captures the key actors involved in conflicts and events that have occurred in Africa, shedding light on their impact on the lives of people. The absence of actor information raises questions about the circumstances surrounding these events. The dataset reveals the prominence of certain actors in specific regions, such as civilians in the Democratic Republic of Congo, protesters in Algeria, and civilians facing conflict repercussions in Burundi.
    

![](https://lh7-us.googleusercontent.com/E5paiHfVilui0CCN-H4Ew37pxKBPnuEpYA0UT3roOgeiBNrDdMKn5kWU-4HLYdNeE9t6tW4dJQL3JDsko-Dj9jFoXpry34bzVMU7UUshxaynpn0WC_cDx5QjKnLnlN4FXxbjukwBPpRyGiFNxyzLtIYAlQ5lklM)

Figure 2: Distribution of Top Event Actors

  


1.  We discovered that the year, 1999 had the highest number of reported deaths, accounting for approximately 39.5% of the total fatalities.
    

  

![A graph of a bar graph

Description automatically generated with medium confidence](https://lh7-us.googleusercontent.com/TEWxdPeWtuTbdfxBgPDRFtbJ4CNZSweQEcmMMr1fjXdwLNKlGCXTLF7zuSL1tMmfxijGlyvjoHVMoU9jNwEZkFF_eVz-3u3j0vNM1-OOC20ohrthyc8C4h7DMC1N8ipxQjMmfuQhey_niijdAZHV3SlrUiNGL7M)

Fig.

2.  Angola emerged as the nation with the most reported deaths, accounting for approximately 35.6% of the total fatalities. Shockingly, we identified that Eastern Africa and Middle Africa have witnessed the highest number of fatalities, with a staggering total of 126,929 and 239,064 respectively. These numbers serve as a stark reminder of the human cost of these conflicts.
    

  

![A graph of different colored barsDescription automatically generated](https://lh7-us.googleusercontent.com/eEoFBf5tf7ynVWYxbEFjUL8QipvOicIDvYxKfF6rFWirfxChiV13fcLHgfpc-Sow8oXJ4y5AK7jEmEp3lLa1VKrHtTNrKUbz4LRCcXmZpdXvKb172X8y2LScLoplQvQ_FEJ_s3ISp6SItXCNp4T4A7pTirin6jg)

![A map of africa with different colored spotsDescription automatically generated](https://lh7-us.googleusercontent.com/dDAb4O18g36A7ImYlcvwXRp7rpDZacVE-BLIaSiuh4OPgkOP3IaXFoZy1fRV4ierW8iAj3iNf4Hz41s0hkFa_CCEEXsYbWdJmLPBNzyFFaTIcjJNuZqm0FyswkVIgQt285Yh1GcpeqVrqx-sB-ugBOtkag-fntU)

Figure 2: Geospatial distribution of Event types by Fatalities

The heatmap reveals the areas with the highest density of conflicts, highlighting the regions that require immediate attention and intervention. This visual representation helps policymakers and organizations identify the hotspots and allocate resources effectively.

![A graph with a bar graphDescription automatically generated](https://lh7-us.googleusercontent.com/0R55t1lw49PgtkYQjnYfQZ73diFXQkl2iNL-0qsJ1QvV948rK8xCYDss-UY1_KjFHrijG6Um1xHxZCCyAuxM04oSM4iSmzdk2FfNueoAvtCv1zReX8r3z2K5BP7-EQ9IcYDQXQ2jIvuIYI-I7aI3ZGlLG-eq7WI) Figure 3: Frequency Distribution of Source Scale Conflict Report

### Model Training

To facilitate the creation and validation of the model, the dataset was divided into two parts: the training dataset and the testing dataset.

### Model Evaluation

During the model evaluation, we employed several supervised machine learning algorithms including Logistic Regression, Nearest Neighbor, Gaussian Naïve Bayes, Decision Tree, and Random Forest Classification. Among these algorithms, Random Forest Classification algorithm demonstrated the best performance, exhibiting the highest accuracy score of 86%.

  
  
  

### Model Validation

The train/test split method was employed to validate the model.

### Model Deployment

GitHub: [https://github.com/Akash190104/Hamoye-Data-Fusion](https://github.com/Akash190104/Hamoye-Data-Fusion)

### Results

  

 ### Conclusion and Recommendation
