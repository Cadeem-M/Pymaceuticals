# Pymaceuticals
As a senior data analyst at Pymaceuticals, I am tasked with comparing the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens. in an attempt to screen for potential treatments for squamous cell carcinoma.



##Closing and credits.

https://www.youtube.com/watch?v=e5oOvU0VWBQ How to Remove Duplicate Rows in Pandas Dataframe? | GeeksforGeeks by GeeksforGeeks



https://stackoverflow.com/questions/73648429/matplotlib-plot-plotting-the-wrong-data-values by use lambda
using x_axis = y_axis.index 


https://www.youtube.com/watch?v=GitXv_t0dZ4 Matplotlib Subplot - How Do You Plot a Subplot in Python Using Matplotlib | Matplotlib Tutorial by WsCube Tech! ENGLISH


AskBCS Learning Assistant - Unathi

# Get the duplicate mice by ID number that shows up for Mouse ID and Timepoint. 
duplicate_mouse_ids = study_data_complete.loc[study_data_complete.duplicated(subset=['Mouse ID', 'Timepoint']),'Mouse ID'].unique().........
duplicate_mouse_ids
