---
layout: default
---

a

## Rush hours being the most problematic

<img align="left" width="500" src="assets/accidents_distribution_static.png" style="padding-right: 20px">
On the left we can see distributions of number of accidents thorughout hours of the day and days of the week. Regarding time of accidents, we can see that there are two peaks: around 7 a.m. and 4 p.m. These are rush hours, when most people are travelling to are from work, so it's self-explanatory that the probability of an accident is higher then. When we look at the distribution over the days of week, we can see that most accidents happen during working days, with a similar number of occurences every day. At the same time, there's a small peak on Fridays - maybe people are tired after a whole week of work and drive less carefully? On weekends there are much less accident - which is also quite obvious, since most people don't work on weekends, making the traffic much less intensive.

<iframe src="assets/weekdays_bokeh.html"
    sandbox="allow-same-origin allow-scripts"
    align="left"
    width="100%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

Now that we saw how many accidents happen within hours of the day and days of week, let's compare distribution of accidents for every weekday. We saw that taking all data into account, most accidents happen during rush hours, but is it like that every single day? What about weekends, when we don't really have the same rush hours? Indeed, when we compare weekends with working days there is a big difference. Weekend has its own rules. Number of accidents is much more steady throughout the day (both on Saturdays and Sundays) - we don't observe such sharp peaks as during working days. Of course, similar as during the rest of the week, more accidents happen during the day than during the night. Traffic incidents are most common between 10 a.m. and 10 p.m.
