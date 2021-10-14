# matplotlib-challenge


# Intro

The purpose of this project was to import, group and compare medical data of a set of Mice undergoing treatments for cancer as a means of testing cancer drugs.
Using Jupyter Notebook, Python,  Pandas, and Matplotlib, we will be running through the core sets of data visualization techniques to demonstrate their utility in analyzing information.

# Data Set 
<mouse_metadata.csv>
<study_results.csv>

 For reasons unknown the data pertaining to the mice was split into a pair of CSV files containing information pertaining to the physical characteristics of the mice themselves and characteristics of potential tumors within the mice over time.

A limitation observed was that the Timepoint variable has no measure to indicate how much time one timepoint pertains to, so while we can use the information to show Tumor characteristics across the Timepoints, the story of the growth(s) will be less accurate.

# Method

The files were merged into one cohesive data frame then cleaned of duplicate entries before any data was pulled for visual comparisons. Afterwards, a summary data frame for the Drug Regiments was made utilizing the mean, median, mode, standard deviation, and standard error functions in python and formatted to three significant figures.

The next plan of action was to move data through different graphs as a means of displaying the data visualization potential of pandas data frames and matplot's graphs with a touch of comparisons between pyplot and matplot. This was done by passing columns of the Clean_DataFrame through functions [ .groupby() &/or .value_counts() ] this allowed us to group the data as desire for comparison and pull values for storing as numbers or strings to make easy x/y labels to match graphs.

For quick reference pyplot is a fantastic means of dropping data into a graph and testing the waters, so to speak. It can produce nearly identical graphs when compared to matplot. However, when it comes down to presentation, the amount of customization that can be incorporated through Matplot allows for much better visualizations. 

# Analysis

Capomulin displayed nice results in lowering the Tumor Volume as the timepoints progressed and because Ramicane shares a correlation pattern, it could be safe to say that Ramicane is also successful in lowering the tumor volume in mice.

I observed a trend in two of the treatment drugs when comparing the Average Weight vs Average Tumor Growth.
1. A strong positive correlation in Capomulin.
2. A strong positive correlation in Ramicane.

This leads me to think that there is a relationship between the weight of the mouse and the tumor growth; the lower the weight of the mouse, the lower the volume of the tumor so there may be a link to the effectiveness of the drug based on the weight of the mouse.

To better display the results in the scatter plot and correlation between Capomulin and Ramicane, I constructed a multi-figure graph near the end, the results are extremely similar showing positive correlations and similar changes in weight and tumor volume.

There was a potential outlier when observing the final tumor volume per drug regiment in the Box & Whisker Plots with the drug - Infubinol.

The placebo acted as a fine control to show no trends in change vs drug treatment regiments.

# Conclusion

Grouping the right information to tell the story of the data was a challenge in some parts of the assignment. Having the .ipynb was helpful for obtaining the logic needed to break the assignment down and accomplish some analysis.

Detailing graphs is also a key element that will take more practice. Displaying data is great but displaying it well is an a major skill that can go far in allowing for connections between information sets.

There are some separate visualizations present in the <resources/visualizations/> folder path. They were generated using the last box of the .IPYNB and provide a bit of infomation on the trends of all drugs present in the drug trial.

