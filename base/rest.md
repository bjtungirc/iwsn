# rest接口
http接口==rest接口，可以认为是别名。http是当前服务端和客户端交互使用最多的协议，是前后端交互的桥梁。
# 必须要会一种web后台
过去的三大框架：`jsp` `php` `asp`  
新时代轻量级后台：`python` `nodejs`  
大放异彩的: `golang`

鉴于三大框架过于臃肿，所以这里以后面三种更为轻量的编程语言展示web后台的用法。
## python
python的后台框架不算少，Django、web2py、flask等。flask的用法较为简单，上手较快。可以[参考这里](http://microfrank.top/flask/)快速上手。
## nodejs
nodejs的后台框架也很出名，Express、Koa都是简单易用的很好的框架，Node-Red也是基于Express的，也可以用来写后台接口。
## go
go的web服务器性能远超前面两个，gin是一个不错的web后台框架。可以[参考](http://microfrank.top/go/)
# 作业：写四个rest接口
分别实现往MySQL中增 删 改 查数据
```
get /user/1
put /user/1 
post /user
delete /user/1
```