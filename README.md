# DataCastle_weibo
DataCastle 比赛代码
比赛是已知发布的微博时间，微博的转发的记录与转发时间， 目的是预测新发布的微博的转发量和转发深度
首先统计深度与转发量的算法就花费了我好几天来写。该算法具体是我先将微博转发数据 按照id进行排序，然后为每个id建立一课树来存储。  此次比赛就用了随机森林一个模型因为这样就不用进行交叉验证了，特征为 时间刻度，预测数据前两天的深度（转发量）之差，第二天与第三天的深度（转发量）之差，第三天与第四天的深度（转发量）之差，三个差值的平均等，粉丝数等，
这个比赛是要预测一个新的对象并不是预测以前所给的对象的数据 因此采用这种方法。
