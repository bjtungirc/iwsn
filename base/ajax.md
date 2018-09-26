# 前后交互与跨域问题
先介绍mvc与前后分离的区别，各自的优缺点。

前后分离设计下，web端与后台进行前后交互，数据需要在前端去请求，拿到数据后，将其通过一定的形式展现到页面上来。

例如：图表的数据请求到之后需要画成图展现出来。
# 跨域问题
什么是跨域问题？  
为什么要设置这个阻碍？  
如何解决？（适当补充下当前普遍使用的nginx反向代理模型）
# 前端的异步请求ajax
早期的JQuery中的`$.ajax` `$.get` `$.post`，最常见的形式如下：
```js
$.get(url,data,function(data){})
```
现代浏览器中内置的`fetch`方法，浏览器演示，想学前端的必须了解，这也是个了解ES6重要模型：Promise 的好机会。

```js
fetch(url[,config]).then(res=>{})
```
`axios`用法和fetch很像，都是Promise系，但是axios更强大，他可以在浏览器和Nodejs后台都能使用（fetch只能浏览器使用）。所以axios还可以用来爬虫。
```js
axios.get(url[, config])
axios.delete(url[, config])
axios.post(url[, data[, config]])
axios.put(url[, data[, config]])
```
# 要求
能用JQuery fetch axios的任意一种交互方式完成与服务端的交互  
# 作业：配合之前的增删改查接口，写一个UI