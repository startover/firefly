Work In Process
==

导航请移步到: http://python-cn.github.io/guide

说明
--

这里只包含等待开发的Todo List. 会尽量更新到最新状态.

有兴趣参与者请使用: [teambition](http://tburl.in/aba6fdf0)去获取最新的任务列表. 防止任务已被认领造成重复.

沟通请使用: [pythoncn-slack](https://pythoncn.slack.com)(需要邀请, 请发邮件到ciici123@gmail.com, 或者联系组内其他成员),
参与开发者才会被通过(slack没有灌水区)，请谨慎加入

## 学习准备

假如你觉得你还没有能力做下面的todo list, 可以先准备以下一些知识, 将来会用到

- react
- oauth2
- select2

英语好的不妨看这个视频教程[http://discoverflask.com](https://github.com/realpython/discover-flask)

PS: 其他的firefly的依赖的列表在这里: http://python-cn.github.io/guide/#/post/used.md

## 集思广益

社区不是我一个人的观点, 需要大家作为一个潜在受众一起思考: 你希望有什么功能. 然后来建新的card, 去完成你认为有价值的任务.

## Todo List

以下是一些定义:

1. 主题 = model里面的Post, 就是一篇文章
2. 评论 = model里面的Comment, 对一篇文章的评论
3. 首页 = 首页显示了文章的列表, 默认按活跃时间排序
4. 单个主题 = 类似/post/post_id/这样的链接. 包含文章正文, 对应评论等

- [ ] 主题的分类model, 早期可以是先插入的一些固定数据,比如devops, web开发, 爬虫..(选项不重要, 要有后台的支持)
- [ ] 主题的分类model的接口. 前端可以通过ajax调用这个url 获得全部的分类信息: 分类id, 分类名, 分类描述
- [ ] 创建主题时候可以通过select2选择分类, 效果类似meta.discourse.org创建主题的分类下拉框效果(可以只是功能, 没有css样式)
- [ ] 创建请求中会带上分类的参数, 后端save的时候会生成含有分类的主题(Post)
- [ ] 首页渲染时, 能获得某主题对应的分类.
- [ ] 用户创建新主题后会使用[Effeckt.css](https://github.com/h5bp/Effeckt.css), 闪到主题列表的最上面
- [ ] 设计阅读量的实现, 就是刷新一下页面, 阅读量就会+1
- [ ] 让每个主题页面(http://web:port/post/post_id/)里面显示出评论的内容.
- [ ] 首页注册和登陆页面的浏览器兼容性(chrome下正常, FF下不正常)
- [x] 注册页面当用户名/密码/邮箱都有正确输入的时候让`注册`按钮变成enable
- [ ] 设计用户个人页面, 只需要包含对应的view, 个人基本信息: 注册源(微博/github/google), 昵称, 头像(使用Gravatar)等，加入时间, 用户id
- [ ] 设计用户设置密码页面, 对应的view, 简陋的模板
- [ ] 设计用户密码找回方案
- [ ] 用户可以设置自己介绍, 坐标(比如北京), 以及个人的站点
- [ ] 用户可以设置github/stackoverflow的地址
- [ ] 用户model, oauth2方案
- [x] 使用sweetalert替代alert
- [ ] follow用户的功能
- [ ] 站内信模型
- [ ] @ 能弹出被@用户
- [ ] @ 的消息能被该用户收到站内信
- [ ] 使用站内信和其他人私聊
- [ ] 首页每个类型都能排序, 比如按分类, 按最热
- [ ] 设计公告位
- [ ] 每当用户发表新的评论, 应该把该主题提到最前(最近活跃)
- [ ] 完成单个主题页面, 样式, 展示评论, 能在评论下发表新评论
- [ ] 能评论其他人的评论
- [ ] 站内信未读 给标志标示
- [ ] 主题内容在首页就可以预览, 可以选择`阅读更多`点到单个主题页
- [ ] 发布主题可以上传图片
- [ ] 单个主题可以看到上传的图片
- [ ] 发布主题可以插入视频url
- [ ] 单个主题可以看到视频
