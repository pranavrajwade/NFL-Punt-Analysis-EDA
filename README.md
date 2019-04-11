# NFL-Punt-Analysis-EDA


## About

NFL ([National Football League](https://en.wikipedia.org/wiki/National_Football_League)) is a proffessional [Ameriacan Football](https://en.wikipedia.org/wiki/American_football) [league](https://en.wikipedia.org/wiki/Sports_league), that usually takes place from early September to December. In American and Canadian football, a punt is a kick performed by dropping the ball from the hands and then kicking the ball before it hits the ground. [follow this link](https://en.wikipedia.org/wiki/Punt_(gridiron_football)) for more information on Punt.   
This notebook I have done Exploratory Data Analysis on Kaggle's NFL Punt Analytics Competition data using R. The competition was hosted to allow competitors to propose specific rule modifications based on the data provided by NFL for all punt plays from the 2016 and 2017 NFL seasons that includes player rosters, on-field position data and video data, including the plays in which a player suffered a concussion. 
I will be using following libraries to manipulation and visulization :
1) dplyr for manipulation
2) ggplot2 for visualization

Here is the [Link to the Kaggle's comeptetion page](https://www.kaggle.com/c/NFL-Punt-Analytics-Competition).  

## Conclusions

Exploratory data analysis on the given data uncovered follwoing interesting insights : 

- Player Activity in case of Injury:
  'Blocked' and 'Tackling' activities were involved in more than 50% of concussion cases.
![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Player%20Activity%20Vs%20Count.PNG)


- Player Partner Activity in case of Injury:
  'Blocked', 'Tackling' and 'Tackled' consists of considerable amount of instances where concussion occured.
  'Other' activity is where Player Impact was with ground, hence no partner activity was recorded. 
  
  ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Player%20Partner%20Act%20Vs%20Count.PNG)
   
- Impact Type and Concussion
  'Helmet to Body' & 'Helmet to Helmet' impacts resulted in almost all the instances where concussion occured.
  
  ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Impact%20Vs%20Count.PNG)

- Primary Imapct Vs Player Activity
  This plot gives a perfect overview of interrelation between Impact Type, Player Activity and Concussion Count.
  
   ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Primary%20Impact%20Vs%20PlayerAct.PNG)

- Day of Week Vs Concussion
  It seems from this table that chances of a concussion occuring on a Thursday are high but very low on a Sunday.
  
   ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Daywise%20Injury%20Table.PNG)
 
- Stadium Type Vs Concussion 
  It was observed that data regarding stadium type was quite noisy. yet, we can see here that the stadium type 'Outside' is quite         frequent in the Concussion instances.
  
   ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Stadium%20Type%20Vs%20Injury%20Table.PNG)
   
 - Temperature Vs Concussion 
   Concussions are more frequent in low temperatures.
  
   ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Temperature%20Vs%20Count%20Density.PNG)
   
 - Formation type Vs Concussion Rates
   Next, formation table gives us specific formation (which was created using ordered player positions of each play, combined togerther), total number of occurances of the formation, concussive plays out of total occurances and Concussion Rates of each formation.
  
   ![Text](https://github.com/pranavrajwade/NFL-Punt-Analysis-EDA/blob/master/NFL%20Pictures/Formation%20Stats.png)
   
   It was found that following formation types were more likely to experience concussions than others with concussion rates 4% and 5% and considerable Total occurances.
   1) 'GL_GR_P_PDL1_PDL2_PDL3_PDR1_PDR2_PLG_PLL_PLS_PLT_PLW_PPR_PR_PRG_PRT_PRW_VLi_VLo_VRi_VRo'
   
   2) 'GL_GR_P_PDL1_PDL2_PDR1_PDR2_PDR3_PLG_PLM_PLS_PLT_PLW_PPR_PR_PRG_PRT_PRW_VLi_VLo_VRi_VRo'
