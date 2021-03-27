# WEB熬测第一个任务

具体思路是：

1. 创建一个servlet
2. 客户端向服务器发送数据
3. 服务端将数据储存起来（存到contentbuffer,一个StringBuffer类型的东西，当然，存起来之前，先将数据转为字符串）
4. 设置响应报文的头部中content-type为json（对应的MIME是application/json）
5. 通过write方法将contentbuffer按字节写到响应报文并发出）