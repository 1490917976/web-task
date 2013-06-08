-----task4
==========
 

微博项目应用建模
                                   

 组长：丰凯利     活动图
              序列图
	          类图
 组员：刘文洒     用例图
                  文档
      黄俊        ppt





系统需求

系统不同参与者的角度 ,可以将其系统功能分为前台与后台两大功能模块。
要求本系统具有以下功能：
	统一友好的操作界面，能保证系统的易用性。
	规范、完善的基础信息设置。
满足上述需求的系统主要包括下面几个模块：


![alt next](http://ww4.sinaimg.cn/mw1024/a0261fbdtw1e56pxxtytvj20cc0620st.jpg "功能图")








图 1.1系统功能需求

2 需求分析
2.1 识别参与者
在微博系统中，需要会员和管理者甚至浏览者的参与。会员有自己的用户名和密码。浏览者可以注册曾为会员。网站需要一个专门的管理者进行日常维护与管理，发送站内消息，对会员发布的消息进行过滤，所以需要有系统管理员的参与。
参与者有会员、浏览者以及系统管理员。
2.2 识别用例
用例图
![alt next](http://ww4.sinaimg.cn/mw1024/a0261fbdtw1e56q7fc3gej20nv0fk0wr.jpg "功能图")
3 静态结构模型
3.1 定义系统对象
管理员，会员，浏览者，对微薄的各种操作。
3.2 定义类图
系统的类图：
 ![alt next](http://ww3.sinaimg.cn/mw1024/a0261fbdtw1e56pvao2f8j20rh0g8mzq.jpg "功能图")

类不是单独一个模块，各个类之间是存在联系。浏览者必须注册之后才能成为会员，管理者是会员的一个特例，会员对微博内容的各种操作，微薄的类之间的关系如上图类图所示
4 动态行为模型
4.1 创建系统时序图
浏览者注册成为会员的时序图：

 ![alt next](http://ww4.sinaimg.cn/mw1024/a0261fbdtw1e56pry23u1j20it0eg0th.jpg "功能图")
会员登录转发微薄的时序图：
 ![alt next](http://ww3.sinaimg.cn/mw1024/a0261fbdtw1e56qejjklaj20o00e7t9u.jpg "功能图")
会员登录查看微薄的时序图：
 ![alt next](http://ww1.sinaimg.cn/mw1024/a0261fbdtw1e56qf4r1i7j20ni0dqt9r.jpg "功能图")
会员登录发表微薄的时序图：
 ![alt next](http://ww1.sinaimg.cn/mw1024/a0261fbdjw1e56ry0b3zoj20n60daq3z.jpg "功能图")
会员登录关注成为别人的粉丝的时序图：
 ![alt next](http://ww2.sinaimg.cn/mw1024/a0261fbdtw1e56qftjyitj20nq0eh3zn.jpg "功能图")
会员登录回复别人评论的时序图：
 ![alt next](http://ww1.sinaimg.cn/mw1024/a0261fbdtw1e56qfzjb1kj20tv0djjsm.jpg "功能图")
会员登录给好友评论的时序图：
 ![alt next](http://ww4.sinaimg.cn/mw1024/a0261fbdtw1e56qfzs9ojj20ri0dpaba.jpg "功能图")
会员登录删除微薄的时序图：
 ![alt next](http://ww1.sinaimg.cn/mw1024/a0261fbdtw1e56qg08cjej20nu0e2ab5.jpg "功能图")
管理员登录管理评论的时序图：
![alt next](http://ww3.sinaimg.cn/mw1024/a0261fbdjw1e56s2m4uxvj20rs0emabi.jpg "功能图")
管理员登录发站内消息的时序图：
 ![alt next](http://ww1.sinaimg.cn/mw1024/a0261fbdjw1e56s2mje43j20sr0duq4d.jpg "功能图")
会员登录管理会员或者浏览者的时序图：
![alt next](http://ww4.sinaimg.cn/mw1024/a0261fbdjw1e56s2mww6uj20rb0emta6.jpg"功能图")


 

4.2 创建系统的活动图
浏览者注册成为会员活动图：

![alt next] (http://ww1.sinaimg.cn/mw1024/8a9dfd75jw1e56r60wa6yj209u0eht8w.jpg "功能图")


(2)会员对微博内容进行各种操作的活动图：
         
如果会员想要发表微博、评论，转发、回复、关注、等操作是，都应先登录，然后进行相应的操作
![alt next](http://ww4.sinaimg.cn/mw1024/8a9dfd75jw1e56r6277e4j20a10du74j.jpg)
![alt next] (http://ww1.sinaimg.cn/mw1024/8a9dfd75jw1e56r61eso2j209t0f1glu.jpg "功能图")
![alt next] (http://ww1.sinaimg.cn/mw1024/8a9dfd75jw1e56r62iq2pj209s0e7mxd.jpg "功能图")
![alt next] (http://ww3.sinaimg.cn/mw1024/8a9dfd75jw1e56r62pde2j20aj0b3dfv.jpg "功能图")
![alt next] (http://ww3.sinaimg.cn/mw1024/8a9dfd75jw1e56rk016w3j20ae0er3yr.jpg "功能图")
![alt next] (http://ww2.sinaimg.cn/mw1024/8a9dfd75jw1e56rk0b84xj209z0fxjrn.jpg "功能图")

管理员活动

 ![alt next](http://ww4.sinaimg.cn/mw1024/8a9dfd75jw1e56r6155m7j209v0e4dfz.jpg "功能图")
 
 ![alt next](http://ww3.sinaimg.cn/mw1024/8a9dfd75jw1e56r61okz9j20890cu3yn.jpg "功能图")
 
 ![alt next](http://ww1.sinaimg.cn/mw1024/8a9dfd75jw1e56r61yljgj209f0dnt8u.jpg "功能图")


5 总结
本文论述了一个基于WEB的微博系统，基本上体现了微博应用的各方面的优点。所设计微博应用系统，主要是微博初步的探讨和设计。在设计过程中，初步了解了UML的优点和先进之处，了解他的可以自动生成代码的功能。
在设计和制作微博的过程中，培养了自己的综合能力和从全局考虑的思想。这个微博系统功能是很强大的，但出于自己水平有限，作为一个微博系统，该项目上有一些不完善和函待改进之处，有好多东西考虑不周，功能模块不是特别的完善。
通过本次课程设计的编写，对本期的课程进行了系统的复习和应用，加深了对书上知识的了解，对web的建模有了一定的认识。

