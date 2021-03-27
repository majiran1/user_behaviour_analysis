# 项目说明
**具体分析步骤以及结果见"User_Behaviour_Analysis.ipynb"**

数据太大，请至官网自行下载：https://tianchi.aliyun.com/dataset/dataDetail?dataId=42

## 项目简介

本项目旨在分析电商用户（以淘宝为例）的用户行为，并在为用户聚类的基础上为着陆页的更新迭代提供一个可行性准则。具体步骤概述如下：

1. 首先进行数据清洗，然后在时间维度以及用户维度两个维度上分别对PV,UV以及用户的行为转化进行解释性数据分析；

2. 接着根据RFM模型为用户打分，根据RFM指标、性别、年龄这三个特征利用K-Means算法对用户群体进行聚类，评估聚类结果后为用户添加标签；

3. 最后在B页面与A页面之间进行A/B Testing：为保证两组用户的同质性，首先根据聚类的结果对用户进行分流，然后针对“转化率”，“点击量”这两个指标分别进行z检验与t检验，并计算出科恩D值，最终做出实验报告。
## 数据说明

- 本项目的数据来源于阿里天池平台。数据来源官网：https://tianchi.aliyun.com/dataset/dataDetail?dataId=42

- 本项目的数据记录了2015年05月11日-2015年11月11日期间每一天每一个淘宝用户的**行为**（点击，收藏，加购，购买），以及这些用户的具体**信息**（性别，年龄）.

本项目共使用了两个表"user_info_format1.csv"(约42万行数据)与"user_log_format1.csv"(约5千万行数据)，每个表字段的具体说明如下：

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210325212027797.png" alt="image-20210325212027797" style="zoom: 50%;" />

<img src="../../../AppData/Roaming/Typora/typora-user-images/image-20210325212044192.png" alt="image-20210325212044192" style="zoom:50%;" />

## 项目目录

 ![image](https://github.com/majiran1/user_behaviour_analysis/raw/master/screenshots/34.jpg)



