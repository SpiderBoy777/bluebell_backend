# 项目介绍：基于Gin框架的论坛项目，包含用户注册、用户登录、发布帖子、为帖子点赞功能。
## 主要技术点：
1.	使用雪花算法为注册用户生成分布式ID
2.	使用Token模式进行用户身份认证，保证同一账号在同一时间只能登录一个设备
3.	使用令牌桶算法进行限流
4.	支持创建帖子并按照创建时间或得分降序从mysql数据库中查询帖子
5.	支持用户对帖子点赞或点踩，从而根据点赞数和帖子创建时间对帖子进行综合得分
