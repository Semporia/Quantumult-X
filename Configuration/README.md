; 20200127_150456

; 20200127_003325

; 20200126_000709

; 20200111_014752

; 20200107_151515

; 断点终结者专为小白定制的一键导入模板

; TG群传送门：https://t.me/MRHXPJ

[general]  
server_check_url= http://www.qualcomm.cn/generate_204  
;geo_location_checker=http://extreme-ip-lookup.com/json/, https://raw.githubusercontent.com/crossutility/Quantumult-X/master/sample-location-with-script.js  

geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/IP_API.js  

;network_check_url=http://bing.com/
;dns_exclusion_list=*.qq.com, qq.com
;ssid_suspended_list=LINK_22E174, LINK_22E175
;udp_whitelist=53, 123, 1900, 80-443
;excluded_routes= 192.168.0.0/16, 172.16.0.0/12, 100.64.0.0/10, 10.0.0.0/8
;icmp_auto_reply=true
[task_local]
30 7 * * * weather_pro.js

# 多合一签到
0 7 * * * all_in_one.js
[dns]
server=114.114.114.114
server=202.141.176.93 
server=202.141.178.13
server=117.50.10.10
server=223.5.5.5
server=119.29.29.29:53
server=119.28.28.28

server=/*.taobao.com/223.5.5.5
server=/*.tmall.com/223.5.5.5
server=/*.alipay.com/223.5.5.5
server=/*.alicdn.com/223.5.5.5
server=/*.aliyun.com/223.5.5.5
server=/*.jd.com/119.28.28.28
server=/*.qq.com/119.28.28.28
server=/*.tencent.com/119.28.28.28
server=/*.weixin.com/119.28.28.28
server=/*.bilibili.com/119.29.29.29
server=/hdslb.com/119.29.29.29
server=/*.163.com/119.29.29.29
server=/*.126.com/119.29.29.29
server=/*.126.net/119.29.29.29
server=/*.127.net/119.29.29.29
server=/*.netease.com/119.29.29.29
server=/*.mi.com/119.29.29.29
server=/*.xiaomi.com/119.29.29.29
;server=/*testflight.apple.com/23.76.66.98
;server=8.8.8.8
;server=/example1.com/8.8.4.4
;server=/*.example2.com/223.5.5.5
;server=/example4.com/[2001:4860:4860::8888]:53
;address=/example5.com/192.168.16.18
;address=/example6.com/[2001:8d3:8d3:8d3:8d3:8d3:8d3:8d3]


#
# static policy points to the server in candidates you manually selected.
# available policy points to the first available server in candidates based on server_check_url(concurrent url latency test will be immediately launched when the policy has been triggered and the policy result is unavailable).
# round-robin policy points to the next server in candidates for next connection.
# ssid policy points to the server depending on the network environment.
#######🐝#######
# Static静态策略指向手动选择候选服务器。
# Available可用性策略指向候选服务器中的第一个可用服务器（并发URL延迟测试将在触发该策略且策略结果不可用时立即启动）。
# Round-robin轮询策略指向下一个连接候选中的下一个服务器。
# SSID策略根据网络环境指向预设服务器。
#

[policy]  
static=🚫 广告拦截, reject, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Advertising.png  
static=🔰 运营劫持, reject, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Hijacking.png  
static=🍎 苹果服务, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Apple.png  
static=🌏 国外网站, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Global.png  
static=💻 国外影视, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/ForeignMedia.png  
static=📽 国内视频, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/DomesticMedia.png  
static=🎱 HBO, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/HBO.png  
static=🍐 Hulu, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Hulu.png  
static=📺 Netflix, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Netflix_Letter.png  
static=🎬 YouTube, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/YouTube.png  
static=🐝 Pornhub, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Pornhub.png  
static=🦁 动画疯, proxy, direct, img-url=https://github.com/A1exInamin/Zure/raw/master/IconSet/Bahamut.png  
static=💡 Spotify, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Spotify.png  
static=📡 华文电视Pro, proxy, img-url=https://raw.githubusercontent.com/A1exInamin/Zure/master/IconSet/5iTV.png  
static=🌵 Speedtest, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Speedtest.png  
static=🦑 蘋果の新聞, proxy, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Lab.png  
static=🐯 TVB,proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/TVB.png  
static=🎸 TikTok, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/TikTok.png  
static=🌟 IPLC, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Star.png  
static=🐷 BGPX, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Pig.png  
static=🇺🇸 USAX, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/United_States_Map.png  
static=🇨🇳 CHINAX, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/China_Map.png  
static=🇯🇵 Japan, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Japan.png  
static=🏳️‍🌈 Taiwan, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Taiwan.png  
static=🇰🇷 Korea, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Korea.png  
static=🇺🇳 Nations, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/China.png  
static=🇸🇬 Singapore, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Singapore.png  
static=🇬🇧 United Kingdom, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/United_Kingdom.png  
static=🇭🇰 Hong Kong, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Hong_Kong.png  
static=🇺🇸 United States, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/United_States.png  
static=🕹 FINAL, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Final.png  
static=🙈 网易云音乐, direct, proxy, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Netease_Music_Unlock.png  
;static=🦒 可用性策略, proxy, direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/Available.png  
;ssid=🐳 SSID策略, proxy, proxy, 一般路由器: proxy, 翻墙路由器: direct, img-url=https://raw.githubusercontent.com/Semporia/Quantumult-X/master/Qure/IconSet/SSID.png  


;static=policy-name-1, Sample-A, Sample-B, Sample-C
;available=policy-name-2, Sample-A, Sample-B, Sample-C
;round-robin=policy-name-3, Sample-A, Sample-B, Sample-C
;ssid=policy-name-4, Sample-A, Sample-B, LINK_22E171:Sample-B, LINK_22E172:Sample-C

#
# Params ”tag“ and ”enabled“ are optional.
# 参数“ tag”和“ enabled”是可选的。
# The default sync interval for all kinds of remote resources is 24*60*60 seconds.
# 远程资源的默认同步间隔为24*60*60秒。
#

[server_remote]  
https://www.caissr.xyz/link/R1ucsNa43aqSg5zY?sub=1&extend=1, tag=菜菜云, enabled=true  
https://dingyue.suying666.info/link/Ek4pv3L4P3udYLeX?sub=1, tag=速鹰, enabled=true  


[filter_remote]  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Advertising.list, tag=🚫 广告拦截, force-policy=🚫 广告拦截, enabled=true  
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/AdRule.list, tag=📵 广告拦截, force-policy=🚫 广告拦截, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Hijacking.list, tag=🔰 运营劫持, force-policy=🔰 运营劫持, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Apple.list, tag=🍎 苹果服务, force-policy=🍎 苹果服务,enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/China.list, tag=🐼 国内网站, force-policy=direct, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/encoreTVB.list, tag=🐯 TVB, force-policy=🐯 TVB, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/HBO.list, tag=🎱 HBO, force-policy=🎱 HBO, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Hulu.list, tag=🍐 HULU, force-policy=🍐 Hulu, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/TikTok.list, tag=🎸 TikTok, force-policy=🎸 TikTok, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Bahamut.list, tag=🦁 动画疯, force-policy=🦁 动画疯, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Netflix.list, tag=📺 Netflix, force-policy=📺 Netflix, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Spotify.list, tag=💡 Spotify, force-policy=💡 Spotify, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/YouTube.list, tag=🎬 YouTube, force-policy=🎬 YouTube, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/Pornhub.list, tag=🐝 Pornhub, force-policy=🐝 Pornhub, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/DomesticMedia.list, tag=📽 国内视频, force-policy=📽 国内视频, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/ForeignMedia.list, tag=💻 国外影视,force-policy= 💻 国外影视, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Global.list, tag=🌍 国外网站, force-policy= 🌏 国外网站, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Speedtest.list, tag=🌵 Speedtest, force-policy=🌵 Speedtest, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Filter/Media/HWTV.list, tag=📡 华文电视PRO, force-policy=📡 华文电视Pro, enabled=true  
https://sub.jiaowoy.top/Rules/Quantumult%20X/NeteaseMusic.list, tag=🙈 解锁网易云音乐, force-policy=🙈 网易云音乐, enabled=true

[rewrite_remote]  

http://cloudcompute.lbyczf.com/quanx-rewrite, tag=lhie1复写, enabled=true  
https://raw.githubusercontent.com/ConnersHua/Profiles/master/Quantumult/X/Rewrite.conf, tag=神机复写规则, enabled=true  

[server_local]  

;shadowsocks=a.example.com:80, method=chacha20, password=pwd, obfs=http, obfs-host=bing.com, obfs-uri=/resource/file, fast-open=false, udp-relay=false, server_check_url=http://www.apple.com/generate_204, tag=Sample-A  
;shadowsocks=b.example.com:80, method=chacha20, password=pwd, obfs=http, obfs-host=bing.com, obfs-uri=/resource/file, fast-open=false, udp-relay=false, tag=Sample-B  
;shadowsocks=c.example.com:443, method=chacha20, password=pwd, obfs=tls, obfs-host=bing.com, fast-open=false, udp-relay=false, tag=Sample-C  
;shadowsocks=d.example.com:80, method=chacha20, password=pwd, obfs=ws, obfs-host=bing.com, obfs-uri=/ws, fast-open=false, udp-relay=false, tag=Sample-D  
;shadowsocks=e.example.com:80, method=chacha20, password=pwd, obfs=ws, obfs-host=bing.com, fast-open=false, udp-relay=false, tag=Sample-E  
;shadowsocks=f.example.com:443, method=chacha20, password=pwd, obfs=wss, obfs-host=bing.com, obfs-uri=/ws, fast-open=false, udp-relay=false, tag=Sample-F  
;shadowsocks=g.example.com:443, method=chacha20, password=pwd, ssr-protocol=auth_chain_b, ssr-protocol-param=def, obfs=tls1.2_ticket_fastauth, obfs-host=bing.com, tag=Sample-G  

[filter_local]  

# 使用规则屏蔽 IP，有可能误伤其他功能或者应用，可以自己抓包缩小 IP 范围
ip-cidr, 203.119.144.0/23, reject, no-resolve
ip-cidr, 203.119.175.0/24, reject, no-resolve
ip-cidr, 106.11.162.0/24, reject, no-resolve
ip-cidr, 47.102.83.0/24, reject, no-resolve

#绕过企业证书过期
host, ocsp.apple.com, 🚫 广告拦截

#讯飞语记-广告拦截
host-suffix, voiceads.cn, 🚫 广告拦截
host-suffix, ads.voiceads.cn, 🚫 广告拦截
host-suffix, bj.imp.voiceads.cn, 🚫 广告拦截
host-suffix, ai.voiceads.cn, 🚫 广告拦截

#TIKTOK-去水印广告拦截
host-suffix, musical.ly, proxy
host-suffix, tiktokv.com,proxy
host-suffix, tiktokcdn.com,proxy
host-suffix, -tiktokcdn-com,proxy
host-suffix, muscdn.com, proxy
user-agent, TikTok*, proxy  
  
#🦑 蘋果の新聞-广告拦截
host-suffix, appledaily.com.hk, 🦑 蘋果の新聞
host-suffix, nxtdig.com.hk, 🦑 蘋果の新聞
host-suffix, nextmedia.com, 🦑 蘋果の新聞
host-suffix, omoplanet.com, 🦑 蘋果の新聞
host-suffix, nxtdig.com, 🦑 蘋果の新聞
host-suffix, crwdcntrl.net, 🦑 蘋果の新聞
host-suffix, polldaddy.com, 🦑 蘋果の新聞
host-suffix, nexage.com, 🦑 蘋果の新聞
host-suffix, appledaily.com.tw, 🦑 蘋果の新聞
host-suffix, twnextdigital.com, 🦑 蘋果の新聞
host-suffix, nxtdig.com.tw, 🦑 蘋果の新聞
host-suffix, branch.io, 🦑 蘋果の新聞  

#📡 华文电视Pro-广告拦截
HOST-SUFFIX, mob.com, 📡 华文电视Pro
HOST-SUFFIX, 5itv.tv, 📡 华文电视Pro
HOST-SUFFIX, ocnttv.com, 📡 华文电视Pro
USER-AGENT, HWTVMobile*, 📡 华文电视Pro
;user-agent, ?abc*, proxy
;host, www.google.com, proxy
;host-keyword, adsite, reject
;host-suffix, googleapis.com, proxy
ip-cidr, 10.0.0.0/8, direct
ip-cidr, 127.0.0.0/8, direct
ip-cidr, 172.16.0.0/12, direct
ip-cidr, 192.168.0.0/16, direct
ip-cidr, 224.0.0.0/24, direct
geoip, cn, direct
final, 🕹 FINAL
  
# 以下为复写部分（含本地野比JS），包括YouTube去开头5S广告、各种JS去广告+破解VIP，需要把对应野比的JS文件放到本机——quantumult X——script目录下即可。野比大佬github库地址如下：https://github.com/NobyDa/Script/tree/master/QuantumultX 

[rewrite_local]  

#京东历史价格
^https?://api\.m\.jd\.com/client\.action\?functionId=(wareBusiness|serverConfig) url script-response-body jd_price.js  
# 使用脚本屏蔽 IP，不生效的需卸载tb重装，使用这个脚本就不需要写规则了（beta）
^https?://amdc\.m\.taobao\.com/amdc/mobileDispatch url script-response-body tb_price.js  
^https://trade-acs\.m\.taobao\.com/gw/mtop\.taobao\.detail\.getdetail url script-response-body tb_price.js  

# 此处用于京东cookie获取，当失效时需要手动登录京东网页版https://bean.m.jd.com/ 签到获取Cookie, 待QX弹出获取成功即可
https:\/\/api\.m\.jd\.com\/client\.action.*functionId=signBeanIndex url script-request-header all_in_one.js  
# 此处用于百度贴吧cookie获取，当失效时需手动登录https://tieba.baidu.com/index.html贴吧获取cookie，待弹出获取成功即可
^https?:\/\/tieba.baidu\.com url script-request-header all_in_one.js  
# 此处用于百度贴吧cookie获取，APP端直接进去，点击”我的”即可
https?:\/\/c\.tieba\.baidu\.com\/c\/s\/login url script-request-header all_in_one.js  
# 此处用于网易云音乐cookie获取，当失效时需浏览器访问并登录:https://music.163.com/m/login 获取cookie，待弹出获取成功即可
^https?:\/\/music\.163\.com url script-request-header all_in_one.js  
# 此处用于爱奇艺cookie获取，加mitm后打开APP，点击“我的”，待弹出获取成功即可
https:\/\/passport\.iqiyi\.com\/apis\/user\/info\.action.*authcookie url script-request-header all_in_one.js  
# 此处用于52破解cookie获取
https:\/\/www\.52pojie\.cn\/home\.php\?mod=space url script-request-header all_in_one.js  
# 此处用于V2EX cookie获取，浏览器打开https://www.v2ex.com/mission/daily ，待弹出获取成功即可
^https:\/\/www\.v2ex\.com\/mission\/daily url script-request-header all_in_one.js  
# 此处用于电信营业厅APP cookie获取
https:\/\/wapside\.189\.cn:9001\/api\/home\/sign url script-request-header all_in_one.js  
# 饿了么Cookie获取, 打开APP,点击我的,点击左上角的签到,进入页面即可
^https:\/\/h5\.ele\.me\/restapi\/eus\/v\d\/current_user url script-request-header all_in_one.js  
# bili大会员（圈x专用
https://api.bilibili.com/pgc/view/app/season url 302 https://bilibili.mlyx.workers.dev/  
https://api.bilibili.com/pgc/player/api/playurl url 302 https://bilibili.mlyx.workers.dev/  

https://api.bilibili.com/pgc/view/app/season url 302 https://bilibili.mlyx.workers.dev/  
https://api.bilibili.com/pgc/player/api/playurl url 302 https://bilibili.mlyx.workers.dev/  
  
#美区抖音  
  
(?<=(carrier|sys)_region=)CN url 307 US  
  
(?<=version_code=)\d{1,}.\d{1}\.\d{1} url 307 13.0.0
  
# Tiktok封区解锁
(.*video_id=\w{32})(.*watermark=)(.*) url 302 $1
  
#解锁Tiktok日、台、港、韩
(?<=(carrier|account|sys)_region=)CN url 307 JP

(?<=(carrier|account|sys)_region=)CN url 307 TW

(?<=(carrier|account|sys)_region=)CN url 307 HK 

(?<=(carrier|account|sys)_region=)CN url 307 KR

# YouTube ADS
^https?:\/\/.+\.googlevideo\.com\/.+&oad url reject-img
^https?:\/\/.+\.googlevideo\.com\/.+ctier url reject-img
^https?:\/\/youtubei\.googleapis\.com\/youtubei\/.+ad_ url reject-img
^https?:\/\/youtubei\.googleapis\.com\/youtubei\/.+log_ url reject-img
^https?:\/\/.+\.youtube\.com\/get_midroll_ url reject-img
^https?:\/\/premiumyva\.appspot\.com\/vmclickstoadvertisersite url reject-img
^https?:\/\/.+\.youtube\.com\/api\/stats\/ads url reject-img
^https?:\/\/.+\.youtube\.com\/api\/stats\/.+adformat url reject-img
^https?:\/\/.+\.youtube\.com\/pagead\/ url reject-img
^https?:\/\/.+\.youtube\.com\/ptracking url reject-img

# 去微博应用内广告 (By yichahucha)
^https?://m?api\.weibo\.c(n|om)/2/(statuses/(unread|extend|positives/get|(friends|video)(/|_)timeline)|stories/(video_stream|home_list)|(groups|fangle)/timeline|profile/statuses|comments/build_comments|photo/recommend_list|service/picfeed|searchall|cardlist|page) url script-response-body wb_ad.js
^https?://(sdk|wb)app\.uve\.weibo\.com(/interface/sdk/sdkad.php|/wbapplua/wbpullad.lua) url script-response-body wb_launch.js

# 去微信公众号广告 (By Choler)
^https?:\/\/mp\.weixin\.qq\.com\/mp\/getappmsgad url script-response-body Wechat.js

# 知乎去广告 (By onewayticket255)
^https://api.zhihu.com/topstory/follow url script-response-body surgezhihufeed.js
^https://api.zhihu.com/topstory/recommend url script-response-body surgezhihurecommend.js
^https://api.zhihu.com/.*/questions url script-response-body surgezhihuanswer.js
^https://api.zhihu.com/market/header url script-response-body surgezhihumarket.js

# 哔哩哔哩动画去广告 (By onewayticket255)
^https://app.bilibili.com/x/resource/show/tab\?access_key url script-response-body bilibiliTab.js
^https://app.bilibili.com/x/v2/feed/index\?access_key url script-response-body surgebilibilifeed.js
^https://app.bilibili.com/x/v2/account/mine\?access_key url script-response-body bilibiliAccount.js
^https://app.bilibili.com/x/v2/view\?access_key url script-response-body surgebilibiliviewrelate.js
^https://app.bilibili.com/x/v2/rank url script-response-body surgebilibilirank.js
^https://api.bilibili.com/x/v2/reply/main\?access_key url script-response-body surgebilibilireply.js
^https://app.bilibili.com/x/v2/show/popular/index\?access_key url script-response-body surgebilibilihot.js

# 抖音去广告去水印 (By Choler)
^https://[\s\S]*\/aweme/v1/(feed|aweme/post|follow/feed)/ url script-response-body Aweme.js
^https://aweme-eagle(.*)\.snssdk\.com/aweme/v2/ url 302 https://aweme-eagle$1.snssdk.com/aweme/v1/

# 酷我音乐SVIP (By yxiaocai)
^https?:\/\/vip1\.kuwo\.cn\/(vip\/v2\/user\/vip|vip\/spi/mservice) url script-response-body Kuwo.js
^https?:\/\/musicpay\.kuwo\.cn\/music\.pay\?uid\=\d+ url 302 http://musicpay.kuwo.cn/music.pay?uid=1

# 小小影视Vip (By Meeta)
https:\/\/ios\.xiaoxiaoapps\.com\/(vod\/reqplay\/|ucp/index) url script-response-body xxys.js
# 启动广告
https:\/\/ios\.xiaoxiaoapps\.com\/getGlobalData url reject

# 爱美剧Vip (原作 Meeta)（官网下载：app.meiju2018.com）
^https?:\/\/mjapp\.\w{1,9}\.com\/index\.php\/app\/ios\/(vod\/show|user\/index) url script-response-body aimeiju.js
# 广告
^https:\/\/www.3ivf\.com\/index\.php\/app\/android\/ads\/index url reject
^https:\/\/mjappaz\.yefu365\.com\/index\.php\/app\/ios\/ver\/index_ios url reject

# 网易蜗牛读书VIP (By yxiaocai and JO2EY)
^https?://p\.du\.163\.com/readtime/info.json url reject
^https?:\/\/p\.du\.163\.com\/gain\/readtime\/info\.json url script-response-body wnyd.js

# 看漫画极速版vip (By HoGer)
^https?:\/\/getuserinfo\.321mh\.com\/app_api\/v5\/getuserinfo\/ url script-response-body kmh.js

# 知音漫客VIP (By mieqq)
^https://getuserinfo-globalapi.zymk.cn/app_api/v5/(getuserinfo|coin_account|getuserinfo_ticket|getcomicinfo)/ url script-response-body Zymh.js

# 网易漫画去开屏广告
^https://api-163.biliapi.net/cover url reject-img

# 香蕉视频VIP (By Meeta)
^https?:\/\/ios\.fuliapps\.com\/ url script-response-body xjsp.js

# 哔哩哔哩番剧开启1080P+
^https?:\/\/api\.bilibili\.com\/pgc\/player\/api\/playurl url script-response-body bilifj.js

# VSCO滤镜VIP
^https?:\/\/vsco\.co\/api\/subscriptions\/2.1\/user-subscriptions\/ url script-response-body vsco.js

# 大片-视频编辑器 VIP
^https?:\/\/api\.vnision\.com\/v1\/(users\/|banners) url script-response-body dapian.js

# 91短视频
^https?:\/\/.+\.(my10api|(.*91.*))\.(com|tips|app|xyz)(:\d{2,5})?\/api.php$ url script-response-body 91.js

# 布丁漫畫（蜜桃漫画）VIP
^https?:\/\/(bd|bdapp|mitaoapp)\.(4008109966|yeduapp)\.(net|com)\/\/index\.php\/api\/User\/userLogin url script-response-body bdmh.js

# 网易考拉 去广告 (By Choler)
^https://sp\.kaola\.com/api/openad$ url script-response-body wykaola.js

# 腾讯新闻 去广告 (By Choler)
^https://r\.inews\.qq.com\/get(QQNewsUnreadList|RecommendList) url script-response-body QQNews.js

# 商店版香蕉视频VIP (By Meeta)
^https?:\/\/apple\.fuliapps\.com url script-response-body xjsp.js

# 用药助手解锁专业版 (By Primovist)
^https?:\/\/(i|newdrugs)\.dxy\.cn\/(snsapi\/username\/|app\/user\/(pro\/stat\?|init\?timestamp=)) url script-response-body yyzs.js

# 优乐美, 小米粒, 彩色直播三合一 解锁收费房
^https?:\/\/(.+)\.(\w{2,3})(:?\d*)\/(api\/public\/\?service=Live\.checkLive$|public\/\/\?service=Live\.roomCharge$|lg\/video\/loadVideoFees\.do$) url script-response-body zhibo.js

# 陆琪讲故事
^https:\/\/www\.luqijianggushi\.com\/api\/v2\/user\/get url script-response-body luqi.js

# WPS Pro
^https://account.wps.cn|com/api/users/ url script-response-body wps.js

# 万象电视直播
#^https:\/\/u\.kanghuayun\.com\/api\/v2\/info url script-response-body wxzb.js

# Gyroscope 解锁 pro (By Maasea)
^https:\/\/api\.gyrosco\.pe\/v1\/account\/$ url script-response-body gyroscope.js

# 水印精灵 vip (By Alex0510)
^https:\/\/api1\.dobenge\.cn\/api\/user\/getuserinfo url script-response-body syjl.js

# 大千视界
^https:\/\/api\.mvmtv\.com\/index\.php.*(c=user.*a=info|a=addr.*vid=.*) url script-response-body dqsj.js

# JibJab解锁pro
^https:\/\/origin-prod-phoenix\.jibjab\.com\/v1\/user url script-response-body jibjab.js

# 南瓜电影4.7.3版 解锁VIP
^https:\/\/(p\.doras\.api\.vcinema\.cn|pay\.guoing\.com)\/(v5\.0\/user\/\d+$|d\/user\/get_user_info) url script-response-body ngdy.js

# Termius 解锁本地pro  (By Maasea)
https:\/\/api\.termius\.com\/api\/v3\/bulk\/account\/ url script-response-body Termius.js

# 小影 解锁Vip (By @hiepkimcdtk55)
^https:\/\/viva\.v21xy\.com\/api\/rest\/u\/vip url script-response-body vivavideo.js

# 滴答清单 pro
^https:\/\/(ticktick|dida365)\.com\/api\/v2\/user\/status url script-response-body DiDaQingDan.js

#彩云天气 Vip
^https:\/\/biz\.caiyunapp\.com\/v2\/user\?app_name\=weather url script-response-body ColorWeather.js

# 驾校一点通 pro
^https:\/\/vipapi\.jxedt\.com\/vip\/check url script-response-body jxydt.js

# Keep 解锁私人课程和动作库 (QX存在bug 该脚本可能无法生效)
^https:\/\/api\.gotokeep\.com\/(.+\/subject|.+\/dynamic) url script-response-body Keep.js

# 扫描全能王 pro
^https:\/\/(api|api-cs)\.intsig\.net\/purchase\/cs\/query_property\? url script-response-body CamScanner.js

# VUE pro
^https:\/\/api\.vuevideo\.net\/api\/v1\/(users\/.+\/profile|subtitle\/prepare) url script-response-body VUE.js

# NiChi 解锁素材
^https?:\/\/mp\.bybutter\.com\/mood\/(official-templates|privileges) url script-response-body NiChi.js

# PicsArt美易 pro
^https:\/\/api\.(picsart|meiease)\.c(n|om)\/users\/show\/me\.json url script-response-body PicsArt.js

[mitm]
# 需要先生成证书,并开启MitM模块才可以
;passphrase =
;p12 =
;skip_validating_cert = false
;force_sni_domain_name = false
;empty_sni_enabled = false
# cookie获取专用,仅获取cookie时使用,不用的时候最前面加个;
hostname = tieba.baidu.com, c.tieba.baidu.com, music.163.com, passport.iqiyi.com, www.52pojie.cn, *.v2ex.com, wapside.189.cn, h5.ele.me,*.googlevideo.com,s.youtube.com,www.youtube.com,youtubei.googleapis.com,api.weibo.cn, mapi.weibo.com, *.uve.weibo.com, mp.weixin.qq.com, api.bilibili.com, app.bilibili.com, *.zhihu.com, aweme*.snssdk.com, *.kuwo.cn, ios.xiaoxiaoapps.com, api*.tiktokv.com, *.musical.ly, *.amemv.com, mjappaz.yefu365.com, p.du.163.com, getuserinfo.321mh.com, getuserinfo-globalapi.zymk.cn, api-163.biliapi.net, ios.fuliapps.com, vsco.co, api.vnision.com, *.my10api.com, bd.4008109966.net, sp.kaola.com, r.inews.qq.com, apple.fuliapps.com, newdrugs.dxy.cn, bdapp.4008109966.net, app101.avictown.cc, api.hlo.xyz, api.ijo.xyz, www.luqijianggushi.com, account.wps.cn, u.kanghuayun.com, api.gyrosco.pe, api1.dobenge.cn, api.mvmtv.com, mitaoapp.yeduapp.com, origin-prod-phoenix.jibjab.com, www.3ivf.com, pay.guoing.com, p.doras.api.vcinema.cn, api.termius.com, mjappaz.yefu365.com, viva.v21xy.com, dida365.com, ticktick.com, biz.caiyunapp.com, api.gotokeep.com, ap*.intsig.net, mp.bybutter.com, api.vuevideo.net, api.picsart.c*, api.meiease.c*., api*.tiktokv.com, api*.musical.ly, api*.amemv.com, *.tiktokcdn.com,trade-acs.m.taobao.com,amdc.m.taobao.com,api.m.jd.com

;skip_validating_cert = false
;force_sni_domain_name = false
;hostname = *.example.com, *.sample.com

# 以下为lhie1证书，如果不需要用到他的证书，可以换成自己的证书。具体方法请自行Google。

passphrase = 4B676386
p12 = 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
