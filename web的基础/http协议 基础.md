# http协议 基础

## http协议

一种用于规定用户在万维网上进行传输数据时的协议。是一种web客户端和服务器通讯时的规则。

## 媒体类型（MIME type）

web服务器会给所有http对象数据附加一个MIME类型，用于规定当前传输的数据的格式，这样当web客户端拿到数据后，才知道这个数据原来是一个什么东西。比如图片，音频，视频等。

## uri 统一资源标识符

有两种形式

- url统一资源定位符 （几乎所有的uri都是url 很少有人用urn）

		例子：
			http://www.baidu.com/logo.png
			协议    主机地址       主机目录下资源
- urn统一资源名
		
		例子：磁力链接
		
		magnet:?xt=urn:btih:CBCDEFGHIJKLMNOPQRSTUVWXYZ12345678
			

## 常见http方法

- GET
- POST
- DELETE
- PUT
- HEAD

## 常见状态码
- 200 ok
- 302 重定向
- 404 无法获取这个资源
- 304 缓存（内容没有修改）

## 报文
- 起始行
	- 说明要做什么／当前发生了一个什么情况
- 首部
	- 对事情进行描述
- 主体
	- 更详细的描述

## ：-）

用户在把url输入到浏览器中后，按下回车后发生的事情：

1. 浏览器从url中解析出主机的名字
2. 从dns服务器中获取服务器的ip
3. 与服务器建立一条tcp连接
4. 发送http报文
5. 收到服务器返回的http报文
6. 关闭连接，显示文档。

