## Unveiling the Links: TripAdvisor Ratings and Extrinsic Factors on Vacation Rentals in British Columbia, Canada.

# Introduction
The purpose of this project was to explore and analyse data from TripAdvisor and Geoapify APIs to gain insights into rental properties in British Columbia, Canada. And also to investigate any discernible relationship between the ratings of these rentals and their proximity to external locations, including tourist sites, activity centres, entertainment spots, water spots, and spa locations.

# Data Collection
The data collected was in respect of:
 - TripAdvisor:  Rental property name, location, rating, Longitude and Latitude coordinates.
 - Geoapify: External locations near each rental included are tourist sites, activity centres, entertainment spots, water spots, and spa locations as well as their Longitude and Latitude Coordinates.
 - Data Integration: Data from TripAdvisor and Geoapify were integrated based on location coordinates. A consolidated dataset was created for further analysis.
  
# Limitations were set to ensure there would be less outliers and more realistic data output.
1. We limited the calculation of review count to 5 reviews as that was the limit in the free option for the API
2. Entertainment spots: We limited the scanning of radius to 10km and 20 Entertainment spots. 
3. Spa Spots: We limited the scanning of radius 10 km and 20 Spa spots.
4. Activity Centers: We limited the scanning of radius to 10km and 40 activity centres.
5. Tourism Spots: We limited scanning of radius to 10km and  40 Tourism spots.
6. We also lmited the data collected on the rental properties to a total poulation of , regardless of ratings but as fairly distributed accross the province as we could obtain.

# Type of Analysis Conducted
Exploratory Analysis:
1. Descriptive Statistics: Statistical summaries and its visualisation was created to understand the characteristics of the rental data (Check Resources Folfer for table and  Images Folder for Bar Chart).
Also the data points was plotted to show how distributed the data was accross the entire province of British Columbia, Canada (Refer to Images folder for plotted Map).
2. Correlation Analysis: Scatter plots were generated to explore potential relationships between rental ratings and the proximity to external locations (Refer to Images Folder for Scatter Plots), then the         Correlation Coefficient (r-value) whose purpose was to measure the strength and direction of a linear relationship between two variables. It ranges from -1 (perfect negative correlation) to 1 (perfect           positive correlation), with 0 indicating no linear correlation.
The P-Value was also computed for the purpose of assessing the probability of observing a correlation as extreme as the one computed from your data, assuming the null hypothesis that there is no correlation.
   
It is important to note that, while the correlation coefficient describes the strength and direction of a relationship, the p-value helps you assess whether this relationship is likely to be due to chance or whether it is statistically significant. Both are crucial in interpreting the results of a correlation analysis and that is why both values were computed.

# Findings and Insights
- The descriptive insights obtained from the analysis of TripAdvisor rental data in British Columbia aimed to provide an initial understanding of the dataset's characteristics.
- The Map showed that the data Rentals were spread across different geographical locations within British Columbia, including urban, suburban, and rural areas. However, concentrations of rentals were observed       in popular tourist destinations and major cities namely Vancouver Island and Vancouver.
- To better understand the data, we develpoed the null and alternate hypothesis as follows to enable us discover specific patterns.
  1.  Relationship between the number of ratings and the average rating value
      Hypothesis: If a vacation rental receives a high number of ratings, then the average rating of the rental is expected to be higher.
      Null Hypothesis: There is no significant correlation between the number of ratings a vacation rental receives and the average rating value. 

  2.  Correlation between the number of entertainment spots and a vacation rental rating
      Hypothesis: If there are more entertainment spots around a vacation rental, then the vacation rental rating is expected to be higher.
      Null Hypothesis: There is no significant correlation between the number of entertainment spots around a vacation rental and the rental's rating

  3.  Is there a correlation between the number of spa spots and a vacation rental’s rating?
      Hypothesis: There is no correlation between the number of spa spots and a vacation rental’s rating. 
      Null hypothesis: There is  a correlation between the number of spa spots and a vacation rental’s rating.

  4.  Is there a correlation between the number of activities (Clubs, community centers) and a vacation rental’s rating?
      Hypothesis: There is no correlation/relationship between clubs/community centers and vacation rental ratings. 
      Null Hypothesis: There is a positive correlation between clubs/community  and vacation rental rating. 

  5.  Is there a correlation between the number of tourism spots and a vacation rental’s rating?
      Hypothesis: There is a correlation between the number of tourism spots and a vacation rental’s rating.
      Null hypothesis: There is no correlation between the number of tourism spots and a vacation rental’s rating.

  - The statistical correlational analysis produced the following results:
 

        Average rating versus review count produed R-value of 0.0176 with a P-value of 0.1932
        Average rating versus number of entertainment spots gave an R-value of 0.0003  with a P-value of 0.8455
        Average rating versus number of spa spots gave R-value of  0.0695  with a P-value of 0.0087
        Average rating versus number of activity centres gave R-value 0.00823  with a P-value of 0.3743
        Average rating versus number of tourism spots gave R-value 0.00215  with a P-value of  0.6502
        Average rating versus number of water spots gave R-value 0.0003  with a P-value of  0.8765
     
    
# The rule of thumb is that for a higher absolute value of the correlation coefficient suggests a stronger linear relationship. Conversely, a statistically significant p-value with a small correlation coefficient might suggest a weak but non-random relationship.

# Therefore we fail to reject the null hypothesis in all cases.

# Conclusions
Based on the resluts above, it we can confidently say that with the weak correlation found proximity to external locations doesn't strongly impact rental ratings.


=======
link to proposal: https://docs.google.com/document/d/1kUnl6Av2m4WT4tr61aMzhTkb4hk4yu_nTW8C0RHNfw4/edit?usp=sharing
link to powerpoint presentation: https://docs.google.com/presentation/d/1Jpz1d2r5ablezRAFjRA0LAx4tn_ZrYidDcDl8xbE1iA/edit#slide=id.p
API Documentation: Access search APIs for no charge and provides Up to 5 reviews and 5 photos per location


