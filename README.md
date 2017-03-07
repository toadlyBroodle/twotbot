# twatbot
A python commandline bot for automating promotion on social media. Scrape social media with custom queries and promote your product to relevant results with a single command. 
- Features
 -Twitter
  -update user status
  -scan twitter for list of custom queries, dump results in local file (scrapeDump.txt)
   -argument options
    -favorite relevant tweets
    -follow original posters
    -reply to relevant tweets with random promotional tweet from file (promoTweets.txt)

## quick setup
- replace twitter credentials (credentials.py) with your app's own
 - <a href="https://www.digitalocean.com/community/tutorials/how-to-create-a-twitterbot-with-python-3-and-the-tweepy-library">a good guide for how to get credentials</a>
- replace promotional tweets (promoTweets.txt) with your own
 - individual tweets on seperate lines
 - each line must by <= 140 characters long
- replace search queries (queries.txt) with your own
 - individual queries on seperate lines
 - <a href="https://dev.twitter.com/rest/public/search">guide to constructing twitter queries</a>

## usage
twatBot.py [-s,--scrape-twitter \<n\> [-a,--favorite] [-o,--follow] [-p,--promote]] [-u,--update-status] [-h,--help]
: where \<n\> is number of tweets to scrape (n\<=200)
