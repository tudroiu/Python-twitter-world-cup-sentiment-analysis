# Python-twitter-world-cup-sentiment-analysis
Twitter Sentiment Analysis if FIFA World Cup 2018 tweets
Documentation:
By: Eduardo Lebron, Vivek Jadon, Kevin Fitzgerald,  and Tudor Udroiu
To run our code you must have all the source files downloaded:
-	 Fifa2.json
-	tweetLocation.csv
-	trainingdataNeg.csv
-	trainingdataPos.csv
-	testdata.manual.2009.06.14.csv
Section one of our code I would recommend running separately to create the JSON file with all the tweets. This will allow you to not go into twitter every time the code is run.  To run this section of code you will need to input your own API key, API secret, Acess token, and Acess token Secret. We used ours during our project to create the fife2.json file. When you pull yours you will likely obtain different tweets as we pulled ours a couple of weeks ago. 
Section two then call on the JSON file you previously created. Ensure you Path matches as ours is currently set up for our machine. Again recommend running this separately to save processing time for our 100,000 itieration loop. This will also help remove spam tweets and then we clean out some common language from tweets pertaining to links and images. 
This will then create a CSV with all tweets and the locations they were sent from if that setting was enabled or show NA if the setting was disabled when the tweets was sent.  
Section 3 cleans the location data and creates player specific subsets of data to be called upon later. 
Section 4 : This new CSV will be again cleaned in section 3 but then we will use 2 CSV files found online to train our NaiveBayes classifier. These are “trainingdataPos.csv” and “trainingdataNeg.csv”. These have a sufficient amount of tweets to property classifer the pos/neg sentiment model. 
Section 5 is then the sentiment analysis and visual representation. Finding our insights. 


