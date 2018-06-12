
# dr2开新服  
#### 1 先登陆监控查看各个逻辑服,数据库的负载情况(这里是以世界服为例)


[查看逻辑服负载](http://52.8.218.102:8081/screen/966?legend=on&cols=1&start=-21600)

[查看数据库负载](http://52.8.218.102:8081/screen/977?legend=on&cols=1&start=-21600)

[国际服国际boss](http://54.67.35.186:2048/client.html)

点击左边的“客户端热更新”<br>
选择对应的渠道， 然后在最下面添加相应的信息；<br>
![test png](https://raw.githubusercontent.com/boom233/img/master/%E5%9B%BD%E9%99%85%E6%9C%8Dboos.png)

填写新区名: 以前开的服加1, <br>
版本:  按照以前的区服设置<br>
node_name: 去要开的logic看<br>
```
$cat release/dr2_logic_ios417/etc/vm.args 
-name dr2_logic_ios417@172.30.0.250
-setcookie dr2_droidhang2015
+K true
-env ERL_MAX_PORTS 1000000
-smp disable
```
