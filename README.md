
Analyzing the data from mouse SCC tumor drug regimen response results.

![image](https://user-images.githubusercontent.com/95774386/222868086-0ae2eaca-9583-49a4-8015-ee3469c902cf.png)


## Role Playing Background Story
I recently joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications, who has begun screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, I've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked me with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked for a top-level summary of the study results.

## Methodology

### Data prep
Merge the mouse_metadata and study_results DataFrames into a single DataFrame. Remove any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use cleaned DataFrame  to display the updated number of unique mice IDs.

### Analysis Criteria
Provide a statistical summary with the row for each drug regimen, and a column for  mean, median, variance, standard deviation, and SEM of the tumor volume.

Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study (one with the Pandas DataFrame.plot() method and the other with Matplotlib's pyplot methods).

Generate two pie charts that show the distribution of female versus male mice in the study.

Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group.

Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen. Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

Then finally plot the linear regression model on top of the previous scatter plot.
