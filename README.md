# Pymaceuticals
In this week's challenge, I am a senior data analyst at Pymaceuticals who is tasked with analyzing the performance of the company’s drug of interest, Capomulin. Specifally, I will be comparing the drug against the other treatment regimens in an attempt to measure Capomulin's effectiveness in treating squamous cell carcinoma.

Using two provided csv files, "Mouse_meta.csv" and "Study_results.csv", I will merge and manipulate the data to generate tables and figures needed to create a technical report as well as, provide a summary of the results.

## Going about the challenge
This week's challenge relied heavily on manipulating data frames, creating graphs and calculating various statistics. So, pandas,matplotlib.pyplot, and scipy.stats were imported into the script to make use of functions needed.

To go about the challenge mainly, the provided csv files were merged into a single data frame and filtered for duplicated data entries. After, I was left with mainly using the columns like "Drug Regimens", "Tumor Volume (mm3)" and "Timepoint" to handle tasks such as:
comparing the mean and variance of tumor volumes across each drug regimen,
comparing and plotting tumor volumes at their final timepoint across selected drug regimen. 

After completing the technical report, an analysis of Capomulin's performance is given.

## Closing and credits.

This week's assignment was fair. Most if not all of it tested applying what was learned in class but I had to thoroughly take my time with this challenge. I had to take several breaks as I would often hit a road block and that required me to comeback with a fresh mind. Some obstacles I could not overcome on my own are:

1) When appending tumorvol_list (a list to store tumor volumes) with data from a filtered dataset, after a lot of debugging, I noticed that the list stored all of the appended data into a single list (series?) inside of my list (a list/series within a list). I thought each appended item would have its own index and that led to numerous errors. I'm not sure if something was coded wrong, but after realizing my list contained another list that had the items I needed, getting to the solution was not so difficult.

2) I was not sure how to go about searching my data for duplicated mice information without running a for loop. After using AskBCS Learning assistant, an assistant named Unathi provided me with sample code below to help me tackle to question:

**Get the duplicate mice by ID number that shows up for Mouse ID and Timepoint. 
duplicate_mouse_ids = study_data_complete.loc[study_data_complete.duplicated(subset=['Mouse ID', 'Timepoint']),'Mouse ID'].unique().........
duplicate_mouse_ids**

