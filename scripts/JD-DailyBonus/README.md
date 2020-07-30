# 京东多合一签到脚本

> 更新时间: 2020.7.29 20:50 v1.34  
> 有效接口: 24+  
> 脚本兼容: QuantumultX, Surge, Loon, JSBox, Node.js  

## 配置 (Surge)

```properties

*************************
【Surge 4.2+ 脚本配置】:
*************************

[Script]
京东多合一签到 = type=cron,cronexp=5 0 * * *,wake-system=1,timeout=20,script-path=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD-DailyBonus/JD_DailyBonus.js

获取京东Cookie = type=http-request,pattern=https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean,script-path=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD-DailyBonus/JD_DailyBonus.js

[MITM]
hostname = api.m.jd.com

```

## 配置 (QuanX)

```properties

*************************
【 QX 1.0.5+ 脚本配置 】 :
*************************

[task_local]
# 京东多合一签到
# 注意此为订阅路径, 请根据实际情况自行调整
5 0 * * * https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD_DailyBonus.js

[rewrite_local]
# 获取京东Cookie. 
# 注意此为订阅路径, 请根据实际情况自行调整.
https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean url script-request-header https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD_DailyBonus.js

[mitm]
hostname = api.m.jd.com

```

## 配置 (Loon)

```properties

*************************
【Loon 2.1+ 脚本配置】:
*************************

[Script]
cron "5 0 * * *" tag=京东多合一签到, script-path=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD-DailyBonus/JD_DailyBonus.js

http-request https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBean tag=获取京东Cookie, script-path=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/scripts/JD-DailyBonus/JD_DailyBonus.js

[MITM]
hostname = api.m.jd.com

```

## 说明


*************************
【 JSbox, Node.js 说明 】 :
*************************

```properties

开启抓包app后, Safari浏览器登录 https://bean.m.jd.com 点击签到并且出现签到日历后, 返回抓包app搜索关键字 functionId=signBean 复制请求头Cookie填入以下Key处的单引号内即可 */  
  
var Key = ''; //单引号内自行填写您抓取的Cookie  

var DualKey = ''; //如需双账号签到,此处单引号内填写抓取的"账号2"Cookie, 否则请勿填写  

   注1: 以上选项仅针对于JsBox或Node.js, 如果使用QX,Surge,Loon, 请使用脚本获取Cookie.  
   注2: 双账号用户抓取"账号1"Cookie后, 请勿点击退出账号(可能会导致Cookie失效), 需清除浏览器资料或更换浏览器登录"账号2"抓取.  
   注3: 如果复制的Cookie开头为"Cookie: "请把它删除后填入.  
   注4: 如果使用QX,Surge,Loon并获取Cookie后, 再重复填写以上选项, 则签到优先读取以上Cookie.  
   注5: 如果使用Node.js, 需自行安装'request'模块. 例: npm install request -g  

```

*************************
【 QX, Surge, Loon 说明 】 :
*************************

```properties

初次使用时, app配置文件添加脚本配置,并启用Mitm后, Safari浏览器打开登录 https://bean.m.jd.com ,点击签到并且出现签到日历后, 如果通知获得cookie成功, 则可以使用此签到脚本。 注: 请勿在京东APP内获取!!!

由于cookie的有效性(经测试网页Cookie有效周期最长31天)，如果脚本后续弹出cookie无效的通知，则需要重复上述步骤。 
签到脚本将在每天的凌晨0:05执行, 您可以修改执行时间。 因部分接口京豆限量领取, 建议调整为凌晨签到。

```

*************************
【 配置双京东账号签到说明 】 : 
*************************

```properties

正确配置QX、Surge、Loon后, 并使用此脚本获取"账号1"Cookie成功后, 请勿点击退出账号(可能会导致Cookie失效), 需清除浏览器资料或更换浏览器登录"账号2"获取即可.

注: 获取"账号1"或"账号2"的Cookie后, 后续仅可更新该"账号1"或"账号2"的Cookie.
如需写入其他账号,您可开启脚本内"DeleteCookie"选项以清除Cookie

```

## 常见问题

1. 无法写入 Cookie

   - 检查 Surge 系统通知权限放开了没
   - 如果你用的是 Safari, 请尝试在浏览地址栏`手动输入网址`(不要用复制粘贴)

2. 写入 Cookie 成功, 但签到不成功

   - 看看是不是在登录前就写入 Cookie 了
   - 如果是，请确保在登录成功后，再尝试写入 Cookie

3. 为什么有时成功有时失败

   - 很正常，网络问题，哪怕你是手工签到也可能失败（凌晨签到容易拥堵就容易失败）
   - 暂时不考虑代码级的重试机制，但咱有配置级的（暴力美学）：

   - `Surge`配置:

     ```properties
     # 没有什么是一顿饭解决不了的:
     cron "10 0 0 * * *" script-path=xxx.js # 每天00:00:10执行一次
     # 如果有，那就两顿:
     cron "20 0 0 * * *" script-path=xxx.js # 每天00:00:20执行一次
     # 实在不行，三顿也能接受:
     cron "30 0 0 * * *" script-path=xxx.js # 每天00:00:30执行一次

     # 再粗暴点，直接:
     cron "* */60 * * * *" script-path=xxx.js # 每60分执行一次
     ```

   - `QuanX`配置:

     ```properties
     [task_local]
     1 0 * * * xxx.js # 每天00:01执行一次
     2 0 * * * xxx.js # 每天00:02执行一次
     3 0 * * * xxx.js # 每天00:03执行一次

     */60 * * * * xxx.js # 每60分执行一次
     ```
