---_task5
=========
  

微博架构设计


                 组员：
                                     贺院超
    								 单红雪



















系统层析:

![alt next](http://ww1.sinaimg.cn/bmiddle/a0261fbdtw1e5a33ebc0jj20co0bwwf5.jpg "功能图")

我们主要应用了层次架构：
七层代理

![alt next](http://ww4.sinaimg.cn/bmiddle/a0261fbdtw1e5a2mw22uuj20gs0dq0td.jpg "功能图")
1、HTML静态化
效率最高、消耗最小的就是纯静态化的html页面，所以我们尽可能使我们的网站上的
页面采用静态页面来实现，这个最简单的方法其实也是最有效的方法。在我们的微博中：
 ![alt next](http://ww4.sinaimg.cn/bmiddle/a0261fbdtw1e5a2mw8typj20fp0a6dga.jpg "功能图")

2、图片服务器分离
大家知道，对于web服务器来说，不管是pache、IIS还是其他容器，图片是最消耗资源的，于是我们有必要将图片与页面进行分离，这是基本上大型网站都会采用的策略，他们都有独立的图片服务器，甚
至很多台图片服务器。对于我们的微博更是此。经常会分享和上传一些图片，这回耗费大量的资源。
3、数据库
MySQL
  冷热分离
  大字段剥离
  简单使用

![alt next](http://ww4.sinaimg.cn/bmiddle/a0261fbdtw1e5a2mwhi4lj20bv07iq3g.jpg "功能图")

4、缓存
缓存类型主要包括共享内存数据、结果数据、热点、索引，聚合数据
数据缓存：
 
 ![alt next](http://ww1.sinaimg.cn/bmiddle/a0261fbdtw1e5a2mwna9qj20eq097t8w.jpg "功能图")

静态缓存：
（1）缓存原则
数据内容类型及渲染方式
页面生成成本
访问量和命中率
更新复杂度
（2）缓存命中率优化
减少冗余存储
忽略 no-cache
良好的URL设计
区分访问者和访问类型

动态应用层：
（1）Apache +PHP组成的WEB服务单元
环境统一配置和管理
按照业务功能划分服务模块儿
代码一致且同步上线
可快速扩展
（2）基于Memcacheq的消息队列系统
扩展消息格式
异常处理
伸缩性










