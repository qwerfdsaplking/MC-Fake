# MC-Fake
A fake news dataset with multiple topics and social context.

The csv files contains 16 columns: news_id, title, url, publish_date, source, text, labels, n_tweets, n_retweets, n_replies, n_users, tweet_ids, retweet_ids, reply_ids, user_ids, data_name

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

