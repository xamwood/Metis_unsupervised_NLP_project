# Natural Language Processing/ Unsupervised Learning Project: 

## Topic Modeling r/selfimprovement

#### Abstract

Marketresearch.com estimated the self-improvement market to be worth $11.3 billion in 2021 and forecasts the market to grow to $14.0 billion by 2025. Currently Baby Boomers make up the majority share of consumers of self improvement services, but Millennials are a growing consumer base with different needs from their parent's generation. The goal of this project is to discover what those new needs might be so that a publishing company could adequately assess if their current offering of self help literature is meeting what consumers are asking for. I do this by taking data from the subreddit r/selfimprovement and using Latent Dirichlet allocation I model which topics users are posting about. 

#### Design

This project comes out of my interest in knowing how the pandemic has changed the way we live our lives. I'm interested in topic modeling how the areas of ourselves we work on has been changing specifically before and after the pandemic. 



### Data

R/selfimprovement is a subreddit community on the popular social media website reddit. It was created in 2008 and has 1.1 million members. The community describes itself as "for those who have questions about how to improve any aspects of their lives, from motivation and procrastination, to social skills and fitness, and everything in between. It is also a subreddit to share your helpful and civil ideas, tips, and advice on how others can improve themselves." The community has a strict rule of only allowing text based posts that can't include video, images, or external links, and it does not allow for any self promotion. The content of these posts can be scraped using snscrape https://github.com/JustAnotherArchivist/snscrape, which neatly returns a json file of separate posts and comments on the site. Using this data I plan on using an unsupervised machine learning approach to determine how one could break down the topics that people are seeking help in, and determine which topics are more popular than others. Given enough time it would be interesting to see how the topics people are posting about change with time. 

#### Algorithms

During the topic modeling stage I found that the LSA and NMF models weren't very interpretable to me, but there are some groups in the LDA model that made considerably more sense. For example the final model parameters I settle on I could see clear topics relating to:

* Learning/Reading
* Relationships
* Work/School
* Mental Health
* Dating
* Careers
* Routine/Sleep
* Social Media

In analyzing the corpus of posts over time I found that the distribution of these topics in the documents didn't change much over time. I attempted to look at changes through two methods, one in which I summed all the topics for each document in a given month and another where I took the dominant topic in each document and looked at the distribution of dominant topics over a month. Both methods of analysis lead to the same relative order of topic importance for the corpus and showed that topic importance didn't meaningfully change over time. 

##### Tools:

* snscrape for post scrapping
* NLTK,regex,sklearn.feature_extraction for text processing
* Pandas for data manipulation and exploration
* Sklearn.gensim for topic modeling
* Matplot lib/seaborn for visualization

#### Communication

For this project I put together a powerpoint presentation with my findings. 