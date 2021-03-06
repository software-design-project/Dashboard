# Supplementary Requirements
## 修订历史

版本  | 日期 | 描述 | 作者
---- | ---- | ---- | ---
V1.0 | 2018-06-10 | 第一份 | lyq

## 简介

该文档记录了未在用例中描述的需求

## 功能性

### 日志管理
服务端需要维护一个持久数据库，以记录用户的各项信息和每个景区的实时信息
### 景区管理
- 服务器需要记录各景区的实时情况，包括景区内实际人数、购票人数等
- 对于新注册的景区，应该及时加入数据库中
- 对于停止营业的景区，服务器应当立刻关闭购买渠道
- 对于即将达到负载极限的景区，即时提醒景区工作人员，做好
- 对于已经达到负载极限的景区，直接关闭购买渠道，并告知工作人员
### 用户管理
- 保留用户的基本信息
- 存储用户的旅游记录，作为下次推荐的参考
- 用户超过一定时限未使用该款小程序，则删除用户记录
### 安全性
- 保证用户信息不泄露
- 维护付款渠道安全

## 可用性
- 支持部分特殊人群，如色盲、听力障碍等
- 支持模糊匹配、退票等各项功能
- 微信小程序规模较小，支持不同型号的手机
- 支持微信和银行卡两种付款方式

## 可靠性
- 减少小程序出错概率，减少代码BUG
- 保证出错可恢复，尤其是付款和订单部分
- 数据库保存用户信息临时备份

## 法律问题
- 安全权：消费者享有人身和财产安全不被侵犯的权利
- 知情权：消费者有知悉其购买、使用的商品或者接受的服务的真实情况的权利
- 选择权：消费者享有选择商品或者接受服务的权利
- 公平交易权：消费者享有公平交易的权利
- 求偿权：消费者在受到人身损害时，依法享有获得赔偿的权利
- 结社权：消费者依法享有成立维护自身合法权益的社会团体的权利
- 受教育权：消费者享有获得有关消费和消费者权益保护方面的知识的权利
- 受尊重权：消费者享有人格尊严、民族风俗习惯得到尊重的权利
- 监督权：消费者享有对商品和服务以及保护消费者权益工作进行监督的权利
