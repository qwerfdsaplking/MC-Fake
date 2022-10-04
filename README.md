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

## Reference
Please cite the paper whenever our dataset is used to produce published results or incorporated into other software:
```
@inproceedings{min2022divide,
  title={Divide-and-Conquer: Post-User Interaction Network for Fake News Detection on Social Media},
  author={Min, Erxue and Rong, Yu and Bian, Yatao and Xu, Tingyang and Zhao, Peilin and Huang, Junzhou and Ananiadou, Sophia},
  booktitle={Proceedings of the ACM Web Conference 2022},
  pages={1148--1158},
  year={2022}
}
```
