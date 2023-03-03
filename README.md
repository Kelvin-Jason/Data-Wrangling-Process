The Wrangle Process
During the wrangle process, there involved three main stages including:

Gathering Data
Assessing Data
Cleaning Data
There after, I worked on the new and combined data set and created a visual.

Gathering Data
This stage involved gathering data from three sources. The first data set was given and so I imported and saved it in our jupyter notebook as csv. This is using the pandas read function. The second data set involved using the request library while with the third one, we had to request access from twitter and use API. For my case, the developers account did not work for me, and so I used other means including the data given by the instructor in the course. After I gathered all the data, it was now time to work on it by assessing and cleaning it. This process was quite technicak for me but an eye opener of how possible and easy it can be to gather data from different sources such as websites.

Assessing Data
This stage was very interesting, assessing data involved doing so visually and programmatically. Assessing data visually involved using .head() commands and looking at how the data is. From this, I could tell the different columns in our different data sets and the common columns that we had. Programmatic assessing involved looking at the statistics, whether there are null rows and so on. I was able to document several issues with our data that affected its quality and also its structure.

The assessed issues were the following:

Quality issues

Eroneous data types such as in the user ids such as tweet_id, in_reply_to_user id and status.

Some columns are not necessary in our data visualization and/or analysis.

Some rating denominators are not equal to 10.

Some rows are retweets.

The entries in names are not consistent as some start with upper case while others lower case..

P1, p2 and p3 columns some begin with lower case.

Some columns have duplicated entries.

The rating columns(rating_numerator and rating_denominator) should be float.

Tidiness issues

ID fields are in the same table as columns containing dog details.

doggo, floofer, pupper, puppo in first data set are in different columns.

Cleaning Data
After assessing the different issues, I went ahead to make a copy of the original dataset before the cleaning. This will help future me as well as other people to have access to the original data.

Thereafter, I began the cleaning process. I began cleaning the completeness issues, then went on to clean the structural issues, and lastly, I cleaned the content issues. Some issues were not dealt with directly as we had already droped the columns while dealing with the structural issues. Some of the key cleaning was to set the None values of the 4 dog stages to np.nan, then I merged the four columns into one, replaced the two names to include separator ',' and lastly I dropped the original 4 columns. I realized that the cleaning process can iterate and cleaning can actually take much time. Next, I merged our dataset using the merge command and on the common column 'tweet_id' and later saved our data in twitter_archive_master.csv

Our dataset was now ready to be worked on. One could now perform more cleaning, do exploratory data analysis or explanatory data analysis. In our case, I went on to the visualization.

Visualization and Insight
The last part of our project was to check for some insights and do at least one visual using the clean data. I was able to gather three insights and one visual. The content of the insights and visual are in a separate doc named act_report.

I am looking forward to learn more on the visuals in the next part of the course.
