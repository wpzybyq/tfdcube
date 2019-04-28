# 用户贷款风险预测

竞赛信息来源[DC竞赛](https://www.dcjingsai.com/common/cmpt/%E7%94%A8%E6%88%B7%E8%B4%B7%E6%AC%BE%E9%A3%8E%E9%99%A9%E9%A2%84%E6%B5%8B_%E8%B5%9B%E4%BD%93%E4%B8%8E%E6%95%B0%E6%8D%AE.html)


# 数据

1. 数据总体概述  

参赛者可用的训练数据包括用户的基本属性user_info.txt、银行流水记录bank_detail.txt、用户浏览行为browse_history.txt、信用卡账单记录bill_detail.txt、放款时间loan_time.txt，以及这些顾客是否发生逾期行为的记录overdue.txt。（注意：并非每一位用户都有非常完整的记录，如有些用户并没有信用卡账单记录，有些用户却没有银行流水记录。）
相应地，还有用于测试的用户的基本属性、银行流水、信用卡账单记录、浏览行为、放款时间等数据信息，以及待预测用户的id列表。

| 数据表 | 数据表说明 |
| :---: | :---:|
| user_info.txt | 用户的基本属性|
| bank_detail.txt | 银行流水记录|
| browse_history.txt | 用户浏览行为|
| bill_detail.txt | 信用卡账单记录|
| loan_time.txt | 放款时间 |
| overdue.txt |是否发生逾期行为|  


2.数据详细描述  
* 用户的基本属性user_info.txt。共6个字段，其中字段性别为0表示性别未知。
* 银行流水记录bank_detail.txt。共5个字段，其中，第2个字段，时间戳为0表示时间未知；第3个字段，交易类型有两个值，1表示支出、0表示收入；第5个字段，工资收入标记为1时，表示工资收入。
* 用户浏览行为browse_history.txt。共4个字段。其中，第2个字段，时间戳为0表示时间未知。
* 信用卡账单记录bill_detail.txt。共15个字段，其中，第2个字段，时间戳为0表示时间未知。为方便浏览，字段以表格的形式给出。
* 放款时间信息loan_time.txt。共2个字段，用户id和放款时间。
* 顾客是否发生逾期行为的记录overdue.txt。共2个字段。样本标签为1，表示逾期30天以上；样本标签为0，表示逾期10天以内。注意：逾期10天~30天之内的用户，并不在此问题考虑的范围内。用于测试的用户，只提供id列表，文件名为testUsers.csv。

# 评分标准
![评分算法](https://github.com/YangYY013/cube/blob/master/game/1c678dd9-073b-4e17-b1a6-49f99445a3a5.png)


