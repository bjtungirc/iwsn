# websocket
网页版套接字（长连接），http是客户端主动发起请求，才能拿到相应的资源，而websocket则可以服务端主动推送。实时性好、资源利用率高。
# H5的ws API
```javascript
var ws = new WebSocket("ws://localhost:1880/echo")

//监听连接成功、连接关闭、连接出错、消息接收事件
ws.onopen=function(e){}
ws.onclose=function(e){}
ws.onerror=function(e){}
ws.onmessage=function(e){}
```
# 服务端的写法
使用node-red演示
# 非原生websocket
- socket.io 演示
- mqtt自带的ws