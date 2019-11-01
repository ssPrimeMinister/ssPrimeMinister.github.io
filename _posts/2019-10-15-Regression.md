---
layout: post
title: Regression Project
---

<a href='https://github.com/ssPrimeMinister/Regression_Project'>This project</a> performed a regression on all the aircraft crash data since 1908. The goal of this project was to see which factors were the most influential in adding to the deaths of each crash (regarded as the percent of people onboard which died, thus the value can be greater than 1 if the crash killed some on the ground). 

The most difficult aspect of the project was cleaning the data, especially dealing with the summary column (which is just a huge string of characters). I decided to break the summary column into the words contained within it. I then chose, based on what I thought would describe the most situations, specific words to included in the regression (shown in the notebook). For example, "shot down" does a good job of explaining many crashes in which the plane was attacked, so I chose to add "shot down" as a predictor variables. 

After conducting the regression, the most correlated values were:  

Boeing 747-412 (aircraft type)

Boeing 767-223ER (aircraft type)

Boeing B-747-258F (aircraft type)

Boeing B-767-222 (aircraft type)

McDonnell Douglas DC-8F-55 (aircraft type)

Bishkek, Kyrgyzstan (location)

New York City, New York (location)

Quito, Ecuador (location)

AECA Cargo (operator)

El Al (operator)

My Cargo Airlines (ACT Airlines) (operator)

United Air Lines (operator)

Amsterdam - Tel Aviv (route)

Boston - Los Angeles (route)

Hong Kong - Bishkek - Istanbul (route)

Quito - Guayaquil (route)

Controls (type of crash)

The y-intercept was 0.8, meaning that approximately 80% of the people onboard died in a crash. 

However, while many extra predictor variables were created in hopes of improving the regression, the variance is very large—meaning the values used to predict the test set are not very well correlated. The main function pseudo-fixes this problem by running the regression multiple times until the R^2 value is greater than or equal to a specified target. But this is not a proper solution. The proper way to fix this problem would be to gather more data on the crash (however, that is not within the scope of the project).

The entire process is explained in much more detail inside the notebook found in the link above.