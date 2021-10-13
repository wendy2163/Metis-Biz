
**The Question**

The project is inspired by the recent [news](https://markets.businessinsider.com/news/stocks/nancy-pelosi-stock-trades-meme-investing-litquidity-paul-pelosi-alphabet-2021-9), where Nancy Pelosi, the house speaker, became the biggest meme in investing. This raises some questions regarding insider trading, followed by people actively copying and following the Pelosi approach. The ability to shift market sentiment towards one or multiple stocks and generating momentum is a powerful weapon and needs close monitoring. It could be a disaster if it falls into the wrong hands. E.g. dogecoin and Elon Musk. 
According to a CMU [research](https://www.scs.cmu.edu/news/2020/nearly-half-twitter-accounts-discussing-reopening-america-may-be-bots), nearly half of the twitter accounts may be bots, the first question I want to address is: how to identify bot accounts? This is an identification problem. My proposed solution is to build a classification model, based on the twitter account activity, classifying it as bot, no bot, or not clear. 

**The Design**

The criteria of success is to lower the % of bot tweets for main companies. It needs to be baseline first, the current percentage of bot tweets in stock related topics. 
The desired impact of this project is to help the SEC monitor market fluctuation, fight insider trading. Further desired impacts include preventing individuals or groups from using social media to cascade propaganda, tracing bots, and detecting fraud. The impact hypothesis is that classifying bot tweets will improve twitter’s credibility, and improve fraud detection. The hypothesis assumes twitter prioritizes content quality over speed, and bot/no bot classification is possible. 

**The Data**

For the preliminary exploratory data analysis, I used the data set from kaggle: [tweets about top companies from 2015 to 2020](https://www.kaggle.com/omermetinn/tweets-about-the-top-companies-from-2015-to-2020/tasks?taskId=2825). The raw data contains three sheets, the main tweet sheet contains over one million records, each row represents an individual tweet, the columns include tweet_id, writer, post_date, body, number of comments, number of retweets and number of likes.
I also have a [data set](https://www.kaggle.com/omermetinn/values-of-top-nasdaq-copanies-from-2010-to-2020) regarding the values of top companies.

**The Algorithms**

I used Natural Language Toolkit to assign each tweet sentiment score, this allows me to represent tweets in a numeric way and conduct analysis based on the positive sentiment and total sentiment score. 


**The Tool** 

I used python and google sheet for data exploration, data blending, data processing. Tableau is used for visualization.
