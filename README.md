# Uber Rides Data Analysis
Importing Libraries
The analysis will be done using the following libraries : 

Pandas:  This library helps to load the data frame in a 2D array format and has multiple functions to perform analysis tasks in one go.
Numpy: Numpy arrays are very fast and can perform large computations in a very short time.
Matplotlib / Seaborn: This library is used to draw visualizations

Importing Dataset

# Data Preprocessing
As we understood that there are a lot of null values in PURPOSE column, so for that we will me filling the null values with a NOT keyword. You can try something else too.

Changing the START_DATE and END_DATE to the date_time format so that further it can be use to do analysis.

Splitting the START_DATE to date and time column and then converting the time into four different categories i.e. Morning, Afternoon, Evening, Night

# Data Visualization
In this section, we will try to understand and compare all columns.

Let’s start with checking the unique values in dataset of the columns with object datatype.
Now, we will be using matplotlib and seaborn library for countplot the CATEGORY and PURPOSE columns.

Most of the rides are booked for business purpose.
Most of the people book cabs for Meetings and Meal / Entertain purpose.
Most of the cabs are booked in the time duration of 10am-5pm (Afternoon).
As we have seen that CATEGORY and PURPOSE columns are two very important columns. So now we will be using OneHotEncoder to categories them


Business and Personal Category are highly negatively correlated, this have already proven earlier. So this plot, justifies the above conclusions.
There is not much correlation between the features.
Now, as we need to visualize the month data. This can we same as done before (for hours)


The counts are very irregular.
Still its very clear that the counts are very less during Nov, Dec, Jan, which justifies the fact that  time winters are there in Florida, US.
Visualization for days data.
Insights from the above plots :
Most of the cabs booked for the distance of 4-5 miles.
Majorly people chooses cabs for the distance of 0-20 miles.
For distance more than 20 miles cab counts is nearly negligible.
