# Udacity-Term-2-Data-Wrangling

Wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations using Python.

Additional data was gathered from Twitter's API

Image in the WeRateDogs Twitter archive was run through a neural network by Udacity that can classify breeds of dogs. 
The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images) are found image predictions file.

This data wrangling process consists of: 
- Gathering data
- Assessing data
-Cleaning data

Finally, storing, analyzing, and visualizing your wrangled data.
Reporting on 1) your data wrangling efforts and 2) your data analyses and visualizations

Gathering Data for this Project
Each of the three pieces of data were gathered as described below in a Jupyter Notebook titled wrangle_act.ipynb:

The WeRateDogs Twitter archive (twitter_archive_enhanced.csv): This file was manually dowloaded.

The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is presented in each tweet according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's servers and was downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

Each tweet's retweet count and favorite ("like") count at minimum, and any additional data was extracted using the tweet IDs in the WeRateDogs Twitter archive, twitter API for each tweet's JSON data was queried using Python's Tweepy library and each tweet's entire set of JSON data were stored in a file called tweet_json.txt file. Each tweet's JSON data was written to its own line. The.txt file was read line by line into a pandas DataFrame. 