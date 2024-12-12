# PHP2550 PDA Project 1: Marathon Performance Analysis

## Summary

This project investigated the relationships between environmental factors, age, and sex in marathon performance across five major U.S. marathons (Boston, Chicago, New York City, Twin Cities, and Grandma's Marathons) from 1993 to 2016. The study analyzed data from 11,564 runners across 98 marathon events to understand how various factors influence completion times. The analysis revealed clear age-based performance patterns, with runners between ages 20-40 demonstrating superior performance compared to other age groups. Male record-breakers clustered in the 21-34 age range, while female record-breakers spanned a broader range of 23-41 years. A U-shaped relationship emerged between age and completion time, with performance declining more steeply at both ends of the age spectrum.

<div align="center">
  <img width="400" alt="spline_plot" src="https://github.com/user-attachments/assets/3521a17f-1776-4a2b-a3ff-5c5a86bc44c1" />
</div>

Environmental conditions emerged as key determinants of marathon performance. The Wet Bulb Globe Temperature (WBGT), which combines temperature, humidity, and solar radiation measurements, showed particular impact on older runners who exhibited greater performance variability under different temperature conditions. 
<div align="center">
  <img width="400" alt="WBGT" src="https://github.com/user-attachments/assets/9fa132af-edd5-4556-89d1-053d3ed196f4" />
</div>
Wind speed demonstrated a gender-specific effect, with female runners showing more resilience to wind variations compared to their male counterparts. 
<div align="center">
  <img width="400" alt="wind" src="https://github.com/user-attachments/assets/016b84c5-df73-46c3-9041-b36c44e94cf6" />
</div>
Statistical analysis using hierarchical random intercept models for both female and male runners revealed that WBGT, wind speed, and PM2.5 levels all showed statistically significant positive correlations with completion times, indicating that challenging environmental conditions generally led to slower performance. Notably, ozone levels, which remained within safe ranges (0-0.054 ppm) throughout the events, did not show a significant impact on marathon completion times. 
<div align="center">
  <img width="400" alt="model_male" src="https://github.com/user-attachments/assets/fd2f5421-b85d-4ce9-9a73-325e21d4bd41" />
</div>
The research contains some limitations due to missing weather data for four marathons (2011 Chicago, 2011 NYC, 2011 TC, and 2012 Grandma's). Future research could strengthen these findings through imputation of missing values and expansion to include more marathons across different geographical regions. These findings provide valuable insights for marathon organizers and runners, highlighting the importance of considering both demographic factors and environmental conditions in race planning and performance expectations. The results suggest that age-specific strategies and environmental adaptations might be particularly beneficial for optimizing marathon performance.

## Files

`project1.qmd`: This file contains R code and text explanations of the Exploratory Data Analysis.

`project1.pdf`: A PDF version of the Exploratory Data Analysis report with Code Appendix at the end

## Dependencies

I used the following packages for this analysis: tidyverse, knitr, tidyr, dplyr, kableExtra, readr, visdat, gridExtra, corrplot, splines, lme4, lmerTest, ggplot2, gridExtra.
