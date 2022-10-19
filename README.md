# MC-Fake
A fake news dataset containing 28334 news events in multiple topics (Politics, Entertainment, Health, Covid-19, Syria War) and corresponding social context (tweets, retweets, replies, users, retweet_relations, replying relations, user-follow-user relations) collected from Twitter.

The dataset can be downloaded from [link](https://drive.google.com/file/d/1WAyOVLqM1JOQdlpsCdKKuRltOGVC9bGt/view?usp=sharing)

The csv files contains 18 columns: news_id, title, url, publish_date, source, text, labels, n_tweets, n_retweets, n_replies, n_users, tweet_ids, retweet_ids, reply_ids, user_ids, retweet_relations, reply_relations, data_name



```
news_id: the ID of the news event
title: title of the news
url: source url of the news
publish_date: publish date
source: news source
text: text content of the news
labels: veracity label of the news
n_tweets: tweet counts
n_retweets: retweet counts
n_replies: reply counts
n_users: user counts
tweet_ids: IDs of the relevant tweets, separated by commas
retweet_ids: IDs of the relevant retweets, separated by commas
reply_ids: IDs of the relevant replies, separated by commas
user_ids: IDs of the relevant users, separated by commas
retweet_relations: retweet relations indicated by a list of tokens {tweet_ID_A}-{tweet_ID_B}-{user_ID of tweet A}-{user_ID of tweet B} denoting A retweets B
reply_relations: reply relations indicated by a list of tokens {tweet_ID_A}-{tweet_ID_B}-{user_ID of tweet A}-{user_ID of tweet B} denoting A replies B
data_name: news category
```

The large user social network file is in 
```
https://ai.tencent.com/ailab/ml/mcfake/edges_all.txt.gz.aa
https://ai.tencent.com/ailab/ml/mcfake/edges_all.txt.gz.ab
https://ai.tencent.com/ailab/ml/mcfake/edges_all.txt.gz.ac
https://ai.tencent.com/ailab/ml/mcfake/edges_all.txt.gz.ad
```
Please use the following cmd to merge all files and then uncompress it.
```
cat edges_all.tar.gz.* > edges_all.tar.gz
```
Each line in the file is in the format of "{userA_ID},{userB_ID}", denoting a "follow" relationship from user A to user B

## Reference
Detailed data construction process and data analysis is in our paper, please cite the paper whenever our dataset is used to produce published results or incorporated into other software:
```
@inproceedings{min2022divide,
  title={Divide-and-Conquer: Post-User Interaction Network for Fake News Detection on Social Media},
  author={Min, Erxue and Rong, Yu and Bian, Yatao and Xu, Tingyang and Zhao, Peilin and Huang, Junzhou and Ananiadou, Sophia},
  booktitle={Proceedings of the ACM Web Conference 2022},
  pages={1148--1158},
  year={2022}
}
```
