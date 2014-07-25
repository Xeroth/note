http://wangcong.org/articles/learning-iptables.cn.html

买了台linode，最近为了玩ingress，搭建vpn是势在必行的事情了。
搭建vpn的时候遇到iptable的转发问题，不搞清楚总觉得胸闷气短的。
是时候搞明白，舒畅一下了。

**iptables 的表和链**

iptables(表\表对应的链)  |1     |2
:------------:|:-------------:| ------------
raw          |PREROUTING     |
mangle       |PREROUTING|FORWARD
nat          |PREROUTING     |
filter       |	INPUT, FORWARD , OUTPUT|


