### Quantumult X BoxJs 在 Mac 上访问

```
[http_backend]

https://raw.githubusercontent.com/chavyleung/scripts/master/box/chavy.boxjs.js, tag=BoxJs.net, path=^/, enabled=false

```

* 设置 HTTP Backend 地址与端口（127.0.0.1:9999）

* 重启 HTTP Backend 模块，重启代理（VPN)  

* 下载 [chavy.boxjs.html](https://raw.githubusercontent.com/chavyleung/scripts/master/box/chavy.boxjs.html) 到 Mac

* 在 iOS 的系统设置里找到自己的局域网地址，如：192.168.50.100

* 双击打开 chavy.boxjs.html 文件

* 在浏览器地址的 URL 地址后面，增加 baseURL 参数

* 在 URL 后面增加：?baseURL=http://192.168.50.100:9999 

* 注意：192.168.50.100 是 QuanX 的局域网地址

* 完整示例：

* file:///Users/username/Downloads/chavy.boxjs.html?baseURL=http://192.168.1.62:9999