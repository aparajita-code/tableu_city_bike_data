

In this assignment, I have created visualizations, dashboards and a story using Tableau for the New York Citi Bike Program. CitiBike is the largest bike-sharing program in the United States.

Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the Citi Bike Data webpage.

This Tableau dashboard is created with the purpose to establish a sophisticated reporting process. The set of visualizations are aimed to provide data reports to the city officials.


Data Preparation :

To extract data for all twelve months from the large CSV files of city bike data for 2023, the extraction has been performed in the terminal using the shell script below

"File: $1" >> 2023_sample_city_bike_data.csv ; head -n 500  "$1" >> 2023_sample_city_bike_data.csv' _ {} \;"

code explained :

find . -type f -name "*.csv": This finds all files (-type f) with the extension .csv in the current directory and its subdirectories.

-exec sh -c 'echo "File: $1" >> output.csv; head -n 10 "$1" >> output.csv' _ {}:

sh -c 'commands' _ {}: Executes the given commands for each file found.

echo "File: $1" >> output.csv: Appends the file name to output.csv to indicate the source of the records.

head -n 500 "$1" >> output.csv: Appends the first ten lines of each CSV file to output.csv.



I have used the  data only for the full year 2023. 
took first 500 samples from each month .
the analysis is based on the chosen number of data samples only .


Tableau Public Link :


Key Insights :




**Questions to Answer:**


In this assignment, I aimed at aggregating the data found in the Citi Bike Trip History Logs and find two unexpected phenomena. The phenomena tha I have chosen are:

Which ride types are the most popular and how do they vary between members and casual riders?

What is the average trip duration and what are the trends for duration for different months, weekdays, and hours?

Setp 1: Create Visualizations
In the first step, I created multiple visualizations to answer the two questions stated above.

Rides

The first step was to compute the total number of rides in 2023 
The next visualization reviews the ride types and their count by Months. This shows that classic bikes are the most used types of bike and they remain dominant through out the year. Next are the electric bikes. And then the trips ondocked bikes are almost negligible.


