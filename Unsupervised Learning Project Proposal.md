### Unsupervised Learning Project Proposal

##### Question/Need:

Marketresearch.com estimated the self-improvement market to be worth $11.3 billion in 2021 and forecasts the market to grow to $14.0 billion by 2025. Currently Baby Boomers make up the majority share of consumers of self improvement services, but Millennials are a growing consumer base with different needs from their parent's generation. The goal of this project is to discover what those new needs might be so that a publishing company could adequately assess if their current offering of self help literature is meeting what consumers are asking for. 



##### Data Description:

R/selfimprovement is a subreddit community on the popular social media website reddit. It was created in 2008 and has 1.1 million members. The community describes itself as "for those who have questions about how to improve any aspects of their lives, from motivation and procrastination, to social skills and fitness, and everything in between. It is also a subreddit to share your helpful and civil ideas, tips, and advice on how others can improve themselves." The community has a strict rule of only allowing text based posts that can't include video, images, or external links, and it does not allow for any self promotion. The content of these posts can be scraped using snscrape https://github.com/JustAnotherArchivist/snscrape, which neatly returns a json file of separate posts and comments on the site. Using this data I plan on using an unsupervised machine learning approach to determine how one could break down the topics that people are seeking help in, and determine which topics are more popular than others. Given enough time it would be interesting to see how the topics people are posting about change with time. 



##### Tools:

* snscrape for post scrapping
* NLTK,regex,sklearn.feature_extraction for text processing
* Pandas for data manipulation and exploration
* Sklearn.decomposition for topic modeling
* Matplot lib/seaborn for visualization



##### MVP Goal:

The MVP for this project will be having the data extracted processed and a basic topic model done.











