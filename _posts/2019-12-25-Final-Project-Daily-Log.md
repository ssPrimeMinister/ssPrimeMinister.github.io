---
layout: post
Title: Final Project Daily Log
---

Below is a log of my daily progress, including:

1.) What I worked on today

2.) What I learned

3.) Any road blocks or questions that I need to get answered

4.) What my goals are for tomorrow

**January 7th**

1.) Today I tried to generalize reading in a CSV file. I have realized that some datasets contain non-UTF-8 characters, thus not allowing pandas to convert it to a dataset.

2.) I learned how to read the bytes of the a file and display them, but I am still trying to test each character (whether it is UTF-8 or not).

3.) All the resources I found to my questions were written in Python 2, so I still need to find a method for Python 3.

4.) My goals are to find a method for testing the characters and generalize a function to remove them. Then, I would like to create other methods for reading in each column.

**January 8th**

1.) Today I discovered a method for eliminating non-unicode characters from a CSV file.

2.) I learned how to deal with non-unicode characters in byte form—they are greater than 128. My questions were mainly surrounding what to do with the bytes of a file when only read in byte-form. Yesterday, I managed to access the byte version of the file with 'rb,' but I didn't know what to actually do with the bytes. After discovering that all unicode bytes are 128 or less, I then only saved the bytes with that restriction. Then, I interpreted those bytes with bytes([b]). Finally, I combined all the remaining lists of single letters and other unicode characters by the commas separating them.

3.) No current roadblocks, I just need to move onto my next goals.

4.) Tomorrow, I hope to comment my code from today and move on to interpreting the datatypes of the columns.

**January 9th**

1.) Today I experimented with different methods for interpreting the column data to the user.

2.) I learning that I need to have a second user input with what the datatypes are.

3.) I am still set on having the least amount of user input as possible, so my roadblocks revolve around eliminating that input.

4.) Tomorrow, I hope to discover a new method for interpreting the data so that the user does not have to specify anything.

**January 10th**

1.) Today, I discovered a new method for interpreting the data for the user—simply asking them if my evaluations are correct (string data or numerical data).

2.) I learned that my largest challenge is going to be working with the categorical data, as it could just look like a bunch of information in strings.

3.) I still am trying to eliminate as much user input as possible, so my biggest roadblock is still the same.

4.) Tomorrow, I am going to move past this issue and begin implementing linear regression (pipelines) into the class.

**January 13th**

1.) Today, while I did attempt to begin implementing the linear regression, I quickly began working on my data interpretation again.

2.) I have discovered a new way to interpret the categorical data. If something is cast as a string (through my interpreter), there are two possible cases: it holds one value or multiple. I believe that the secret to automating the categorical interpretation is in the length of the inputs.

3.) I am still trying to parse out categorical information with names longer than one string (like ["Airbus," "A380"]).

4.) I plan to continue to work on this interpretation section for the first thirty minutes then implementing regression for the last thirty minutes.

**January 15th**

1.) Today I began to implement the linear regression and some natural language processing.

2.) I discovered that about three inputs in a column is usually a categorical variable, so I will use that estimate to find all possible categorical columns

3.) I ran into an issue with the linear regression. For polynomial features, I have to somehow find the lowest intersection of bias and error without viewing the graph. Again, I do not want any user input, so this will be slightly complicated.

4.) I will work on finding the intersection of the bias and error without user input.

**January 16th**

.) I stumbled upon something that was killing my kernel: MultiIndexing. Thus, all my work today was devoted to fixing that error.

2.) I did not even know MultiIndexes exist. As I found out, when I was converting each column to either an integer or a string, I used to_numeric instead of astype(float). I thought that they would produce the same thing but, as I discovered, they do not. When I was casting a column to a float with to_numeric, I was adding an index inside of a column. That is to say, each row had an index, as they always do, but each entry in a specific column also had an index specific to that column. However, because I didn't change any of the indices, the internal column index was the same as the row index. But, nevertheless, it seemed my kernel could not handle trying to covert this MultiIndex to a one hot category.

3.) No roadblocks right now, I solved my problem by using astype instead of to_numeric

4.) My goals for the weekend are to successfully implement the regression systems. I do not see this as being too difficult, as I have already done projects with each (so I will just have to figure out a way to make them generalizable).

**January 17th**