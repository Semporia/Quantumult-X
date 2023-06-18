# BoxJs 在 Mac 上访问

**Quantumult X**

```
[http_backend]

https://raw.githubusercontent.com/chavyleung/scripts/master/box/chavy.boxjs.js, tag=BoxJs.net, path=^/, enabled=false

```

* 将 A、B 两台设备置于同一局域网内

* 【A设备】使用 HTTP Backend 的方式来配置 BoxJs

* 【A设备】设置 HTTP Backend 的监听地址为 0.0.0.0，端口默认 9999 即可  

* 【A设备】通过自身浏览器访问 http://127.0.0.1:9999 验证是否正常访问

* 【A设备】取得本设备的局域网地址，如：192.168.x.x

* 【B设备】打开浏览器并访问：http://192.168.x.x:9999 即可
