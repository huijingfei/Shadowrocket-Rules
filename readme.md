### 自用iOS Shadowrocket规则

fork自 Johnshall 的白名单规则，适量精简，加入部分app广告屏蔽规则。

在原白名单规则的基础上，逐渐完善手机端APP的分流规则；因本规则属于个人自用，如有覆盖不到的地方请联系我。

Johnshall白名单规则:

------------------------------------------------------

    https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever

------------------------------------------------------

自用规则：

------------------------------------------------------

    https://raw.githubusercontent.com/huijingfei/shadowrocket/main/sr_app_ad.conf

------------------------------------------------------
    
    直连：top500 网站中可直连的境外网站、中国网站
    
    代理：默认代理其余的所有境外网站


------------------------------------------------------

GeoLite2数据库：

    https://raw.githubusercontent.com/Hackl0us/GeoIP2-CN/release/Country.mmdb

------------------------------------------------------

## 规则使用方法

方法一：用 ShadowRocket 扫描二维码即可。

![二维码](https://raw.githubusercontent.com/huijingfei/shadowrocket/main/QR%20Code/shadowrocket.png)

方法二：在 ShadowRocket 应用中，进入 [配置] 页面，点击右上角加号，将规则文件地址粘贴到 url 处，点击“下载”即可。

## 规则更新频率
不定时更新

## iOS中屏蔽应用开屏广告的方法：
设置→屏幕使用时间→内容和隐私访问限制→Apple广告→不允许
