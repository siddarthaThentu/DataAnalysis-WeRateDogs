**What is this project about**
- In this project, we look at ways to gather data, supplement the incomplete data by wrangling the required data from the internet thorugh API, manually download available data files. After that, we assess the data for issues in it's quality and tidiness. Then, we clean the issues and save the clean file.

**Libraries Used**
- pandas : data manipulation
- numpy : numerical manipulation
- requests : downloading data from the internet
- re : extracting the regular expressions
- tweepy : downloading data through twitter API
- json : handling json format data
- timeit : calculate the time taken

**Steps Taken**
- Data gathering
- Data assesing
- Data cleaning
- Data analysis

**Case Study**
<br><br>
<a href='https://twitter.com/dog_rates'>WeRateDogs</a> is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage. In this case study, we currently have **two pieces of data/dataframes available with us**. Let's take a minute to explore them.
 <br>
 
 1. Through Udacity, we have access to a few tweet data provided by WeRateDogs. However, this data has only basic features like 'tweet_id','dog_name','retweet_id' etc. Some important features like the number of retweets and number of favorites (which show the popularity of the dog) were not provided. Luckily, with the given tweet_id's, we can wrangle this tweets from WeRateDog's archive and extract the required content.<br><br>
    **Name : twitter-archive-enhanced-2.csv** <br>
    **Source : <a href="https://www.udacity.com/">Udacity</a>**<br>
    **Access : manual download from website**
 <br><br>
 
 2. Each tweet in the twitter-archive-enhanced-2.csv is thought to have images of the dog. These images were fed into a Dog breed classifier model to identify the type and breed of dog. This was done by the Udacity team and the file was hosted on Udacity's server.<br><br>
    **Name : image-predictions.tsv** <br>
    **Source : <a href="https://www.udacity.com/">Udacity</a>**<br>
    **Access : Download the file from server through requests library**

<h1>Files</h1>

 - wrangle_act.ipynb : Entire code for the project
 - act_report.html : Medium blog post explaining the visualizations
 - act_report.pdf : A pdf report of the  blog post
 - wrangle_report.pdf : A report identifying the steps taken during the stages of data analysis
 - twitter-archive-enhanced.csv : Data that we are starting with.
 - tweets_json.txt : Tweet data extracted through tweepy API and stored in a text file
 - image_predictions.csv : Predictions for dog names from the image urls
 - twitter_archive_master : Final data after cleaning
