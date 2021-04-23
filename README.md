# News

## 看点新闻

### 基本描述
看点新闻App通过获取互联网专业数据科技服务商---聚合数据的新闻接口来实现新闻数据的展示。由于每日限制100次请求，故每次请求时就缓存新闻数据到本地数据库中。当每次下拉刷新就分页查询10条新闻数据重新显示在对应的tab碎片中。用户可以根据自己的兴趣点击对应的tab标签来阅读新闻，清除本地缓存，登录后（取消）收藏新闻，查看个人收藏，添加、查看、删除个人发布的文章等

### 系统功能描述
**登录、注册模块**：注册过的用户登录后才能（取消）收藏新闻，查看个人收藏，添加、查看、删除个人发布的文章等。
**个人信息模块**：用户登录后可以查看、修改个人资料。
**个人文章模块**：用户登录后可以发布、查看、删除文章。
**个人收藏模块**：用户登录后可以（取消）收藏新闻接口数据子项，并且查看自己收藏的所有新闻。
**清除缓存模块**：该功能主要清除浏览网页时在本地留下的离线内容和图片缓存。
**展示新闻列表模块**：该功能主要在用户打开App时，就请求聚合数据提供的新闻接口来显示在tab页面并将请求的数据缓存到本地数据库中。若当日请求次数已用完，则分页查询本地数据库。


## 关键技术
使用AsyncTask+LitePal+分页查询异步更新每个tab页面数据；使用GSON解析格式化JSON接口数据；充分引用Material Design界面设计规则的依赖库来优化UI；使用递归算法计算文件（目录）大小和删除文件（目录）；使用LitePal数据库存储技术；使用Fragment碎片来作为每个tab页面；使用ListView布局、RecycleView布局来显示新闻列表。
