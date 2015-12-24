# golang匿名聊天室 支持@定向消息

本实例基于websocket和jQuery开发。
[websocket](https://github.com/gorilla/websocket)
[jQuery](http://jquery.com)

本实例特点如下：
1. 支持浏览器客户端和命令行客户端两种方式。
2. 支持私聊。

## 运行实例

实例运行运行在go环境中，安装go环境请参照(http://golang.org/doc/install)

启动服务器。

    $ go get github.com/gorilla/websocket
    $ git clone git@github.com:innger/gochat.git
    $ cd server
    $ go run *.go

运行命令行客户端

    $ cd client
    $ go run *.go

运行浏览器客户端
    http://127.0.0.1/

登录聊天室：

	访问即登录，随机分配用户名，即可开始聊天

跟某人私聊输入：

    @dengyanlu 私聊信息

后端 goroutine + chan 支持高并发
