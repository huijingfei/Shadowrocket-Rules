# 自用iOS Shadowrocket规则

🛑 fork自 Johnshall 的白名单规则。
🛑 精简部分国外小语种网站。
🛑 完善欧美主流网站规则。
🛑 加入部分app广告屏蔽规则。

在原白名单规则的基础上，逐渐完善手机端APP的分流规则；因本规则属于个人自用，如有覆盖不到的地方请联系我。

## Johnshall白名单规则:

------------------------------------------------------

    https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever

------------------------------------------------------

## 自用规则：

------------------------------------------------------

    https://raw.githubusercontent.com/huijingfei/shadowrocket/main/sr_app_ad.conf

------------------------------------------------------
    
    直连：top500 网站中可直连的境外网站、中国网站
    
    代理：默认代理其余的所有境外网站


------------------------------------------------------

## GeoLite2数据库：

------------------------------------------------------

    https://github.com/Loyalsoldier/geoip/releases

------------------------------------------------------

## 规则使用方法

方法一：用 ShadowRocket 扫描二维码即可。

![二维码](https://raw.githubusercontent.com/huijingfei/shadowrocket/main/QR%20Code/shadowrocket.png)

方法二：在 ShadowRocket 应用中，进入 [配置] 页面，点击右上角加号，将规则文件地址粘贴到 url 处，点击“下载”即可。

## 规则更新频率

根据日常使用不定时更新

## 自用V2rayN自定义规则

直接下载[V2rayN-Rule-Whitelist.json](https://raw.githubusercontent.com/huijingfei/shadowrocket/main/V2rayN-Rule-Whitelist.json)，导入V2rayN路由设置即可。


## V2Ray 路由规则文件

[v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)可代替 V2Ray 官方 geoip.dat 和 geosite.dat。
