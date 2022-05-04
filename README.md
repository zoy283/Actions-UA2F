
## 一个云编译UA2F固件的项目
###### 来自MoorCorPa/Actions-immortalWrt-UA2F，添加了SSR-PLUS,经测试运行正常

* 如果要自己设置规则记得把
<br><code>iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN</code>
* 改成以下规则
<br><code>iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN</code>


### 食用方法：
##### 用其他设备的话请改Main.config里的上面三行，改成自己所需要的 config，复制别人的来用也行，下面的不要动哦
##### aciton务必使用Main

<br><a href="http://trac.gateworks.com/wiki/OpenWrt/kernelconfig">参考文献</a><br>
<a href="https://sunbk201public.notion.site/sunbk201public/OpenWrt-f59ae1a76741486092c27bc24dbadc59">详细教程</a><br>
<a href=“https://github.com/Zxilly/UA2F”>UA2F</a><br>
