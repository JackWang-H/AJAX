# HTTP
HTTP（hypertext transport protocol）协议【超文本传输协议】，协议详细规定了浏览器和万维网服务器之间互相通信的规则

## 请求报文(四部分)
重点是格式与参数
```
行 （包括三部分）	请求类型:GET/POST     路径/参数 URL  /s？ie=utf-8   协议版本HTTP/1.1

头  格式：名字: 值
    HOST: blog.sliber.cn
    Cookie: name=LMK
	Content-type: application/x-www-form-urlencoded
	Uer-Agent: chrom 83    
空行（空行是必须有的）
体   username=admin&password=admin
```
响应报文
```
行（包括三部分）	协议版本：HTTP/1.1    响应状态码（*404 *403 *401 *500 *200）   响应状态字符串OK
头	Content-Type: text/html;charset=utf-8
	 Content-length: 2048
	 Content-encoding: gzip

空行
体  （HTML内容放在响应报文体中）  
    <html>
		<head>
		</head>
		<body>
			<h1>ajax学习</h1>
		</body>
	</html>
```
