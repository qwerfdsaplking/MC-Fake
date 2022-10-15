# MC-Fake
A fake news dataset with multiple topics (Politics, Entertainment, Health, Covid-19, Syria War) and social context (tweets, retweets, replies, users, retweet_relations, replying relations, user-follow-user relations).

The csv files contains 16 columns: news_id, title, url, publish_date, source, text, labels, n_tweets, n_retweets, n_replies, n_users, tweet_ids, retweet_ids, reply_ids, user_ids, data_name

```
news_id: the id of the news event
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
tweet_ids: IDs of the relevant tweets
retweet_ids: IDs of the relevant retweets
reply_ids: IDs of the relevant replies
user_ids: IDs of the relevant users
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
