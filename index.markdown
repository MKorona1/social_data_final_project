---
title: Title
layout: default
---

California is one of the states in the US with the largest total number of car accidents according to [World Population Review](https://worldpopulationreview.com/). It also has a largest numbeber of traffic fatalities as per [CDC](https://www.cdc.gov/nchs/pressroom/sosmap/accident_mortality/accident.htm). Even though the mortality rate per 100,000 population isn't among the highest ones, the problem still seems to be quite serious, especially that up until 2023, number of traffic fatalities was consistently increasing according to [TIMS](https://tims.berkeley.edu/summary.php#). [SafeTREC Berkely](https://safetrec.berkeley.edu/2023-safetrec-traffic-safety-facts-speeding-related-and-other-crashes) informed that, in 2021, 35% fatalities were speed-related, compared to 29% nationwide, which seems to be one of the main causes of severe car accident in California. Taking this into account, it seems strange that California state introduced their first speed cameras only at the beginning of 2024 in the trail run, according to [The New York Times](https://www.nytimes.com/2023/10/13/us/california-speed-cameras.html). In this analysis we try get insights into traffic accidents' patterns in California, taking into account factors like time and location of occurence, or weather conditions, and understand what else can be done to prevent accidents from happening.

## Rush hours being the most problematic

<img align="left" width="500" src="assets/accidents_distribution_static.png" style="padding-right: 20px">
On the left we can see distributions of number of accidents thorughout hours of the day and days of the week. Regarding time of accidents, we can see that there are two peaks: around 7 a.m. and 4 p.m. These are rush hours, when most people are travelling to are from work, so it's self-explanatory that the probability of an accident is higher then. When we look at the distribution over the days of week, we can see that most accidents happen during working days, with a similar number of occurences every day. At the same time, there's a small peak on Fridays - maybe people are tired after a whole week of work and drive less carefully? On weekends there are much less accident - which is also quite obvious, since most people don't work on weekends, making the traffic much less intensive.

<iframe src="assets/weekdays_bokeh.html"
    sandbox="allow-same-origin allow-scripts"
    align="left"
    width="100%"
    height=550
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

Now that we saw how many accidents happen within hours of the day and days of week, let's compare distribution of accidents for every weekday. We saw that taking all data into account, most accidents happen during rush hours, but is it like that every single day? What about weekends, when we don't really have the same rush hours? Indeed, when we compare weekends with working days there is a big difference. Weekend has its own rules. Number of accidents is much more steady throughout the day (both on Saturdays and Sundays) - we don't observe such sharp peaks as during working days. Of course, similar as during the rest of the week, more accidents happen during the day than during the night. Traffic incidents are most common between 10 a.m. and 10 p.m.

We already know when traffic accidents usually happen - let's see what are the most problematic locations in California.



## Exploring Locations of Serious Accidents in California
California boasts diverse climates, vast geographical features, and various densely populated areas, which correspondingly influence the occurrence of traffic accidents.

Understanding where serious accidents frequently occur is crucial for planning accident prevention strategies.

To this end, we have created a heatmap based on California's accident data, where areas with higher severity are marked in darker colors. This heatmap reveals that serious accidents are particularly concentrated in the Los Angeles area. Notably, the Los Angeles region, with its high population density and heavy traffic, faces an increased risk of traffic accidents.

<iframe src="assets/losangeles_heatmap.html"
    sandbox="allow-same-origin allow-scripts"
    align="left"
    width="100%"
    height=550
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

To further refine our analysis, we focused on data from within the city of Los Angeles, particularly identifying locations around highway entrances and exits where serious accidents frequently occur.

Our analysis specifically highlighted the Santa Monica Freeway (Interstate 10) in Los Angeles. This freeway stretches approximately 17 miles east-west from Santa Monica to downtown Los Angeles. It is one of the areas with the highest frequency of accidents in Los Angeles.

The high frequency of accidents on I-10 can be attributed to its intersections with other major freeways—I-5, I-110, and I-405. These intersections complicate traffic flow and, with numerous exits in succession, often force drivers to make frequent lane changes. Such conditions demand high concentration from drivers and increase the likelihood of accidents due to distractions.

Moreover, this area experiences almost non-stop traffic 24 hours a day, and visibility worsens during bad weather, further increasing the risk of accidents. Therefore, during peak traffic times and adverse weather conditions, drivers need to exercise even greater caution.


## The Relationship Between Weather Conditions, Time of Day, and the Severity of Accidents

<img align= "middle" width="500" src="assets/weather condition.png" style="padding-right: 20px">

In traffic safety, weather significantly impacts driving conditions. Our analysis categorizes fifteen frequently occurring weather conditions into five major groups. This categorization helps us understand how different weather conditions influence the severity of accidents. Here are the classifications and their rationale:

- Fair Weather Conditions: Clear, Fair, Fair / Windy, Scattered cloud
- Cloudy Conditions: Mostly Cloudy, Cloudy, Overcast, Partly Cloudy
- Wet Conditions: Heavy Rain, Rain, Light Rain
- Slippery Conditions: Light Snow
- Reduced Visibility Conditions: Haze, Fog, Smoke

Our analysis indicates that the severity of accidents at night under slippery and reduced visibility conditions tends to be relatively low. This could be due to drivers being more cautious at night or avoiding driving altogether in severe weather, thus reducing overall traffic volume. Conversely, under clear, cloudy, and rainy conditions, poor visibility at night can lead to increased distraction and higher accident severity. This observation highlights the need for enhanced safety measures and driver awareness during adverse weather conditions, especially at night.


<img align= "middle" width="500" src="assets/county_counts.png" style="padding-right: 20px">


California's diverse geography and extensive road network make it susceptible to various traffic incidents. Examining the distribution of accidents across the state provides valuable insights into patterns and potential risk factors. The southeastern side of California, particularly counties like Riverside, San Bernardino, and Imperial, exhibits a notably higher concentration of accidents, attributed to factors such as population density, transportation infrastructure, and urbanization. Kern County, located in the southern Central Valley, stands out with a relatively high number of accidents due to its strategic transportation routes, while Mono County experiences fewer accidents due to its remote and mountainous terrain. 
