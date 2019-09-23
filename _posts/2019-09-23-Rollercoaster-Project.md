---
layout: post
title: Rollercoasters
---

<a href='https://github.com/ssPrimeMinister/Rollercoaster/blob/master/Lydia%20Zhang%20and%20Hayden%20Nelson%20-%20Roller%20Coaster%20Project.ipynb'>This project</a> dealt with categorizing and evaluating rollercoasters. The goal was to discover interesting facts about different rollercoasters around the world and evaluate them based on set criteria (either set by the user or to a default).

<img src="/images/coaster.png" alt="Inversions vs. Speed" width="500" class="center"/>


<i>Image above is a simple graph showing the correlation between speed and the number of inversions. It is clear that a high speed is associated with little to no inversions, and lower speeds have higher numbers of inversions</i>.

I was responsible for creating a set of criteria by which to evaluate the rollercoasters. In the beginning, I planned to fill the missing data with the average of the column. But after seeing multiple rollercoasters come up in the personalized top ten rollercoasters file after adjusting the criteria (simply because they had many missing values, so the averages significantly helped them), I decided to fill the missing data with 0. Not only did this fix the consistent top ten rollercoasters, but it also created a much more reliable top ten. After we set our own criteria and received our top ten rollercoasters, we wanted to allow the user to specify their preferences. Thus, we allowed the user to allocate 100 points to 8 characteristics. These “points” would become the coefficients in the ranking algorithm.  Changing the missing values from the mean to 0 meant that if, for example, one really desired high G Force (set the G Force factor to 100 and the rest to 0), their results would only contain rollercoasters with actually high G Forces and not filled-in averages. We understand that we penalized the rollercoaster with many missing values, but we feel the user will receive better recommendations as a result.