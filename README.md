# 20-Tableau
Citibike has collected ride data starting in 2013 through present day. For this project I am using data from the month of August for the years 2013, 2016, 2019. My assumption is that August would ridership would be high providing many data points. I also wanted to evaluate the change over time in citibike usage splitting the data into 3 periods. 

# Required Libraries
<ol>
    <li>Pandas</li>
    <li>SqlAlchemy</li>
    <li>sqlalchemy_utils</li>
</ol>
You must also have Jupyter notebooks installed and PostgreSQL.

# The Data
The files used to complete this homework can be found on the Citibike website. They were too large to save to the repository and must be downloaded.
The following files were used for this project:
<ol>
    <li><a href = "https://s3.amazonaws.com/tripdata/201308-citibike-tripdata.zip">August 2013 Tripdata</a></li>
    <li><a href = "https://s3.amazonaws.com/tripdata/201608-citibike-tripdata.zip">August 2016 Tripdata</a></li>
    <li><a href = "https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip">August 2019 Tripdata</a></li>
</ol>

These files must be saved to the file titled Resources in the repository. 

# Data clean up
<ul>
    <li>Run the `Citibank Data Munging.ipynb` file found in the `Jupyter` Folder.</li>
    <li>Be sure to enter your Postgresql password where prompted in the notebook</li>
</ul>

After running Jupyter Notebook Open the "Citibike_Sql.twb" Tableau file. Open the Data Source tab at the bottom then click on the drop down in the upper left for "localhost" and choose "edit connections". Enter your postgres password and click the refresh image at the top of the screen. 


# Tableau Data

In Tableau you should see a series of visualizations along with two dashboards and a story.

## Growth dashboard

<img  src="https://github.com/UncleBacon/20-Tableau/blob/master/Images/Growth_Dashboard.PNG">

The Growth Dashboard shows a steady increase in customers over the three timepoints choosen. There is an overall 50% year over year increase in total customers with Subscribers accounting for a majority of the customer base. The 30-49 year old age group makes up the largest group of subscribers followed by the 50-64 year old age group. This makes sense as these two groups would make up the majority  of the work force and have the income to allow them to subscribe to this service.


## Users Dashboard
<img  src="https://github.com/UncleBacon/20-Tableau/blob/master/Images/Usertypes.gif">

This dashboard shows the how average number of rides and trip durations differ by user types (Customer or Subscriber) and age groups (Subscriber only). Number of rides is dispayed along the vertical axis, average trip duration is indicated by line thickness.

The data shows a clear difference in usage by customers and subscribers. Customers tend to use the bikes throughout the day, peaking in the early to mid afternoon hours. You could make the assumption these users are typically tourists as they do not have a subscrption and tend to use the bikes throughout the day. 

Most subscribers clearly utilize the bikes for travel to and from work and/or school. Usage for the 30-49 and 16-29 year old age groups peak between 7AM to 9AM then again between 4pm to 6pm. This trend is also observed with the 50-64 year old age group but not as strongly. The 65+ age group does not account for a large number of riders however this age group uses bikes conistently throughout the day.

An interesting thing to note is that both customers and the 16-29 year old age group tend to have longer trip durations in the early hours of the morning, between 1 and 4 AM.

## Story Board
<img src = "https://github.com/UncleBacon/20-Tableau/blob/master/Images/Story.gif">

This visualizaiton shows similar data as the <strong>Growth Dasboard</strong> but adds some extra interaction in the form of buttons with prepopulated questions the data can show. 
