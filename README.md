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
