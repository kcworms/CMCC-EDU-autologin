CMCC-EDU-autologin is a script for solving the captive portal of CMCC WLAN(only for SSID:CMCC-EDU).
It supports logging in,showing remaining time(optionally).
It works in a university located in Jinhua,Zhejiang Province,China.

这是一个用来登录CMCC WLAN（仅支持SSID为“CMCC-EDU”的接入点）的脚本。
它支持登录和剩余时间提醒。
它在浙江省金华市某大学测试通过（其实也是在这里写的）。

**(Only python3 now)/(暂时只能工作在Python3下)**
Usage/使用方法
----

Time Reminder enabled:
```
t.py username password remind
```
Time Reminder disabled:
```
t.py username password
```
Cookie will be saved when successfully login the first time.When failed logging in by cookie,it will fallback to no-cookie login method.

----

启用剩余时间提醒:
```
t.py username password remind
```
禁用剩余时间提醒:
```
t.py username password
```
第一次成功登陆时会保存Cookie。当用Cookie登录失败时会使用无Cookie的登录方式。
Automation/自动化
----
Using the Scheduled task of Windows,you can login automatically when you connect to CMCC-EDU.see this [page](http://superuser.com/questions/262799/how-to-launch-a-command-on-network-connection-disconnection).
But logout can only be done manually.

借助Windows的计划任务功能，你能在成功连接至CMCC-EDU后自动登录。