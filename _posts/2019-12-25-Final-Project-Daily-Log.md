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

2.) I learned how to deal with non-unicode characters in byte form—they are greater than 128. My questions were mainly surrounding what to do with the bytes of a file when only ready in byte-form. Yesterday, I managed to access the byte version of the file with 'rb,' but I didn't know what to actually do with the bytes. After discovering that all unicode bytes are 128 or less, I then only saved the bytes with that restriction. Then, I interpreted those bytes with bytes([b]). Finally, I combined all the remaining lists of single letters and other unicode characters by the commas separating them.

3.) No current roadblocks, I just need to move onto my next goals.

4.) Tomorrow, I hope to comment my code from today and move on to interpreting the datatypes of the columns.

**January 9th**

**January 10th**

**January 13th**

**January 15th**

**January 16th**

**January 17th**