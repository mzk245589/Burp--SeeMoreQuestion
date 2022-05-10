# Burp--SeeMoreQuestion
一个被动扫描的Burp小插件
# 介绍

这是一个BurpSuite插件-SeeMoreQuestion。

采用被动扫描的方式，来监听所有经过BurpSuite代理的数据包（无需拦截），根据其请求包和响应包内容来判断其是否存在通用型漏洞或敏感信息。可在浏览目标网站时，打开代理和插件，在遇到敏感时会自动发现显示。

# 使用方式

先打开插件开关

![截图](74dd7d5ee31249e3bc8c506395ba63d4.png)

再浏览网页即可。

![截图](b620b25e88f1ff608333946d853e6558.png)

![截图](47003a7caf734321fb175dd5bf5ece6f.png)

目前被动扫描有：

- 根据remember字段，判断shiro框架
- 根据后台字段，判断敏感信息
- 根据fastjson字段，判断fastjson库
- 根据默认密码或初始密码，判断敏感信息
- 根据.action字段，判断Struts2框架

作者会经常对其进行更新，同时会逐渐优化，减少误报。
