# wechat_recommend_robot
基于Seq2seq、SVD、Native Bayes实现微信聊天推荐机器人

效果视频：



数据算法处理：
1、泊松分布的Native Bayes训练实现输入语句分类:
   [演员推荐方式、电影名推荐方式、闲聊] =  [0,1,2]
2、Seq2seq+Attention机制、细胞单元Cell:双向LSTM                  
   编码-解码 question-answer问答
3、SVD实现降维[电影，用户]矩阵降维
  皮尔逊系数计算构建[电影，电影]相关系数

开发环境python3.6 sdk：
absl-py==0.7.1
astor==0.7.1
numpy==1.16.2
protobuf==3.11.4
tensorboard==1.6.0
tensorflow-gpu==1.6.0
tqdm==4.31.1
Werkzeug==0.15.2
sk-learn==0.0
jieba==0.42.1
itchat==1.3.10
pandas==1.0.3
scipy==1.4.1
