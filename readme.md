## 手动维护的 iOS 小火箭 Shadowrocket 规则 / V2rayN 规则 / V2rayA 规则 (白名单规则) 

小火箭配置文件指的是访问网站需要直连还是代理的规则，例如访问腾讯阿里抖音等网站直连，访问谷歌脸书等走代理。网上一些自动生成的规则具有局限性，例如一些图片视频链接不在规则内，导致一些国内网站或者 APP 访问速度慢，错误的走了代理，在代理线路不好的时候尤其明显，所以才有了这个手动更新的规则。本白名单规则手动更新，时间不固定，专注于改善 APP 体验的小火箭规则。

🛑 精简部分不常访问的小语种网站。

🛑 精简部分垃圾广告域名。

🛑 完善欧美主流网站规则。

🛑 加入部分 APP 广告屏蔽规则。

🛑 完善部分手机 APP 的分流规则。

🛑 更改默认 DNS 为支持 DOH/DOT 的国际大厂 DNS。

🛑 添加常用 SSL 证书域名。

部分广告规则需要开启 https 解密，点击使用的配置文件后的感叹号 i → HTTPS解密 → 开启HTTPS解密 → 点击证书授权，并点击允许 → 前往手机的设置，不是Shadowrocket的 → 看到已下载描述文件 → 安装 → 输入手机的解锁密码 → 安装 → 安装 → 前往手机的设置 → 通用 → 关于本机 → 证书信任设置 → 找到 Shadowrocket 点绿它以信任该根证书 → 继续

### Johnshall 小火箭规则:

------------------------------------------------------

    https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever

------------------------------------------------------

### 自用小火箭规则：

------------------------------------------------------

    https://raw.githubusercontent.com/huijingfei/Shadowrocket-Rules/main/sr_app_ad.conf

    
直连：top500 网站中可直连的境外网站、中国网站
    
代理：默认代理其余的所有境外网站


------------------------------------------------------

### GeoLite2 数据库：

[https://git.io/GeoLite2-Country.mmdb](https://git.io/GeoLite2-Country.mmdb) 数据比较全，文件较大。

[Country-only-cn-private.mmdb](https://raw.githubusercontent.com/Loyalsoldier/geoip/release/Country-only-cn-private.mmdb) 文件较小，只包含 GEOIP,CN 和 GEOIP,PRIVATE。

如果没有特殊需求，使用 [Country-only-cn-private.mmdb](https://raw.githubusercontent.com/Loyalsoldier/geoip/release/Country-only-cn-private.mmdb) 即可。

### 规则使用方法

方法一：用 ShadowRocket 扫描二维码即可。

![二维码](https://github.com/huijingfei/Shadowrocket-Rules/blob/main/QR%20Code/shadowrocket.png?raw=true)

方法二：在 ShadowRocket 应用中，进入 [配置] 页面，点击右上角加号，将规则[文件地址](https://raw.githubusercontent.com/huijingfei/Shadowrocket-Rules/main/sr_app_ad.conf)粘贴到 url 处，点击“下载”即可。

![手动维护的 iOS 小火箭 Shadowrocket 规则](https://github.com/huijingfei/Blog_Gitalk/raw/main/Images/Shadowrocket%20rules.webp)

### 部分 APP 无法使用代理访问解决方法

将相关域名加入跳过代理，建行生活有效，其他未测试。网络环境变化需开关代理一次（例如从 WIFI 换成数据网络），否则仍将提示无法使用代理访问。

    www.baidu.com： 网上国网、多看阅读、顺丰金融、广东农信、丰云行、中国银行缤纷生活、通信行程卡app、趣智校园、趣听音乐、光大手机银行、掌上12333、沃视频
 
    yunbusiness.ccb.com： 建行生活
 
    wxh.wo.cn： 沃小号
 
    gate.lagou.com： 拉勾招聘
 
    www.abchina.com.cn： 中国农业银行
 
    www.shanbay.com  扇贝单词消息中心
 
    www.google.com  成都公积金
 
    login-service.mobile-bank.psbc.com,mobile-bank.psbc.com： 中国邮政储蓄银行

### 自用V2rayN自定义规则

直接下载[V2rayN-Rule-Whitelist.json](https://github.com/huijingfei/Shadowrocket-Rules/releases)，V2rayN路由设置中从文件导入即可，或者直接复制txt文件中的规则，然后在V2rayN路由设置中从剪切板导入。

### V2Ray 路由规则文件

[v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)可代替 V2Ray 官方 geoip.dat 和 geosite.dat。
