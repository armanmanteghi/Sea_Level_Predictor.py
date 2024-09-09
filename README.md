Description of the Code
This Python script analyzes and visualizes global average sea level changes using data from epa-sea-level.csv. It performs the following tasks:

Imports Libraries:

pandas is used for data manipulation and analysis.
matplotlib.pyplot is used for creating plots and visualizations.
scipy.stats.linregress is used for calculating the line of best fit and statistical measures.
Load the Dataset:

The dataset, epa-sea-level.csv, is loaded into a pandas DataFrame named df. This dataset contains information about sea level changes over time, with columns for the year and the adjusted sea level.
Create a Scatter Plot:

A scatter plot is created with the Year column on the x-axis and the CSIRO Adjusted Sea Level column on the y-axis. This plot visualizes the sea level data points.
Calculate and Plot the Line of Best Fit (1880-2050):

The linregress function computes the slope and intercept for the line of best fit using all the data from the dataset.
A line is then plotted representing this best fit line, extending from the earliest year in the dataset to 2050. This line is displayed in red with a dashed style to differentiate it from other plots.
Filter Data for Recent Years (2000-2050):

The dataset is filtered to include only records from the year 2000 onwards. This subset is used to calculate a new line of best fit.
The linregress function is again used to determine the slope and intercept for the best fit line based on this filtered data.
Plot the Line of Best Fit for Recent Years:

A new line is plotted for the recent data, extending from the year 2000 to 2050. This line is displayed in green with a solid line style.
Customize Plot Appearance:

Labels for the x-axis (Year) and y-axis (Sea Level (inches)) are added.
A title (Rise in Sea Level) is set for the plot.
A legend is included to distinguish between the scatter plot and the two lines of best fit.
Save and Display the Plot:

The plot is saved as sea_level_rise.png using plt.savefig().
The plot is then displayed using plt.show().
This visualization helps in understanding the trend of sea level rise over time and provides predictions for the year 2050 based on different time periods: the entire dataset and the recent years since 2000.
