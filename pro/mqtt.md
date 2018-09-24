# mqtt
mqtt是物联网协议，本质是个订阅发布模型的消息队列。这里简单解释下订阅发布。
# mqtt服务安装
emq官网下载解压即可，通过bin/emqttd来启动。默认监听端口有：
```
18083 web管理页面
1883 tcp端口
8883 tcp+ssl端口
8083 ws端口
8084 wss端口
```
演示web端连接和使用
# mqtt客户端使用
可以参考[这里的代码](https://github.com/sunwu51/mqttdemo)