# 京东多合一签到脚本

> 更新时间: 2020.7.18 17:20 v1.29 
> 有效接口: 24+  
> 脚本兼容: QuantumultX, Surge, Loon, JSBox, Node.js  



## 配置



*************************
  
  1、监控github仓库的commits和release。  
  2、监控具体的文件或目录是否有更新。  
  3、新增：可以监控多层目录里面的某个文件  
 
  更新地址：https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/GitHub/GitHub.js  
  配置方法：
  1. 填写github token, 在github > settings > developer settings > personal access token 里面生成一个新token（无需任何权限）。  
  默认TOKEN用的是我自己的，请不要请求过于频繁，每天一两次即可。例如：cron "0 9 * * *"* 2. 配置仓库地址，格式如下：  

  ```properties
  {
    name: "",//填写仓库名称，可自定义  
    file_names:[],//可选参数。若需要监控具体文件或目录，请填写路径（具体看下面示例）。  
    url: "" //仓库的url  
  }
  ```

  📌 如果希望监控某个分支的Commit，请切换到该分支，直接复制URL填入；  
  📌 如果希望监控Release，请切换至Release界面，直接复制URL填入；  





## 配置 (QuanX)

