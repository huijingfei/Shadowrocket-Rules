## 自定义 iOS Shadowrocket 白名单规则 / V2rayN 规则文件

初期 fork 自 Johnshall 的白名单规则，经过长时间的更新，现在与 Johnshall 的白名单规则已有很大差别。本白名单规则手动更新，时间不固定，

🛑 精简部分不常访问的小语种网站。

🛑 精简部分垃圾广告域名。

🛑 完善欧美主流网站规则。

🛑 加入部分 APP 广告屏蔽规则。

🛑 完善部分手机 APP 的分流规则。

🛑 更改默认 DNS 为支持 DOH,DOT 的国际大厂 DNS。

🛑 添加常用 SSL 证书域名。

部分广告规则需要开启 https 解密，不同于网上其他的教程，需要生成新的 CA 证书，使用本规则直接安装证书即可。其中 iOS 系统设置中信任 Shadowrocket 证书的几个步骤不可省略。

### Johnshall 白名单规则:

------------------------------------------------------

    https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever

------------------------------------------------------

### 自用规则：

------------------------------------------------------

    https://github.com/huijingfei/Shadowrocket-Rules/raw/main/sr_app_ad.conf

------------------------------------------------------
    
    直连：top500 网站中可直连的境外网站、中国网站
    
    代理：默认代理其余的所有境外网站


------------------------------------------------------

### GeoLite2 数据库：

------------------------------------------------------

    https://github.com/Loyalsoldier/geoip/releases

------------------------------------------------------

### 规则使用方法

方法一：用 ShadowRocket 扫描二维码即可。

![二维码](https://github.com/huijingfei/Shadowrocket-Rules/blob/main/QR%20Code/Shadowrocket%20rules%20QR%20code.webp?raw=true)

方法二：在 ShadowRocket 应用中，进入 [配置] 页面，点击右上角加号，将规则文件地址粘贴到 url 处，点击“下载”即可。


### 自用V2rayN自定义规则

直接下载[V2rayN-Rule-Whitelist.json](https://github.com/huijingfei/Shadowrocket-Rules/releases)，V2rayN路由设置中从文件导入即可，或者直接复制txt文件中的规则，然后在V2rayN路由设置中从剪切板导入。

### V2Ray 路由规则文件

[v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)可代替 V2Ray 官方 geoip.dat 和 geosite.dat。

### 部分 APP 无法使用代理访问解决方法

将相关域名加入跳过代理，建行生活有效，其他未测试。网络环境变化需开关代理一次（例如从 WIFI 换成数据网络），否则仍将提示无法使用代理访问。

🛑 www.baidu.com： 网上国网、多看阅读、顺丰金融、广东农信、丰云行、中国银行缤纷生活、通信行程卡app、趣智校园、趣听音乐、光大手机银行、掌上12333、沃视频
 
🛑 yunbusiness.ccb.com： 建行生活
 
🛑 wxh.wo.cn： 沃小号
 
🛑 gate.lagou.com： 拉勾招聘
 
🛑 www.abchina.com.cn： 中国农业银行
 
🛑 www.shanbay.com  扇贝单词消息中心
 
🛑 www.google.com  成都公积金
 
🛑 login-service.mobile-bank.psbc.com,mobile-bank.psbc.com： 中国邮政储蓄银行
