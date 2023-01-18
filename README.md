# Data_Anaalysis_Nanodegree
Data_Analysis_Projects
### Quality
1. There are features with extremely high missing values in are 'in_reply_to_status_id', 'in_reply_to_user_id', 'retweeted_status_id','retweeted_status_user_id', 'retweeted_status_timestamp'. These columns have above 92% missing values twitter-archive-enhanced data set.
- Also The column 'expanded_urls' has 2.50% missing values in twitter-archive-enhanced data set

2. The text column contain  multiple variables such as texts, numbers and url links within each single row in twitter-archive-enhanced data set

3. we can also see that the name column in twitter-archive-enhanced data set has object name 'None' (this is could be missing value which have been replace with a value None) thus they will not appear as missing but as object.

4. We can see text column has mixed lower and upper case, while other rows have upper case only and others lower case only in the twitter-archive-enhanced data set.

5. Special characters (punctuation) are also dominant in text column of twitter-archive-enhanced data set.

6. The data type for Timestamp column in twitter-archive-enhanced dataset appears as object instead of datetime dtype

7. The data type of tweet_id is integer and should be object in twitter-archive-enhanced dataset.

8.  We can see the types of dogs such as 'doggo', 'floofer', 'pupper', 'puppo' have more 'None' values implying they have many missing values in twitter-archive-enhanced dataset
9. The name column contain some uncommon values (dog names) such as a , an which neeed to be investigated well(since they might be parts of strings from elsewhere) in twitter-archive-enhanced dataset
10. The source column is a bit dirty with HTML format with a and \a tags surrounding the text (should be cleaned to be more readable)
11. retweeted_status_timestamp column in twitter_archive dataset depicts that the there 181 retweets which may not be neccessary for analysing dogs images

### Tidiness
1. Since 'doggo', 'floofer', 'pupper', 'puppo' columns are  dogs stage they should in a same column name (one variable) and not separate  columns
2. Since the image_predictions dataset has  common column (tweet_id) with twitter_archive dataset thus the two tables need to be merged
