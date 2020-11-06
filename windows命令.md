secpol.msc  本地安全策略管理控制平台

mstsc 打开远程桌面命令

gpedit.msc  本地策略组

nslookup 用于查询DNS的记录，查询域名解析是否正常，在网络故障时用来诊断网络问题 

ipconfig /all 查看所有信息

ipconfig /flushdns 清除dns本地缓存

regedit 注册表

netsh interface show interface  查看有几个网卡

netsh interface ip set address "inside" static 192.168.1.2 255.255.255.0  静态配置网卡ip

netsh interface ip set address "nihao" dhcp 动态分配ip地址

netsh interface ip set dnsserver "nihao" dhcp  动态分配dns地址

netsh interface ip set address "inside" static 8.8.8.8  静态配置dns地址

whoami /user  查看sid

net user 查看所有用户

net user 用户名  查看指定用户的信息

net user 用户名 /active:yes 指定用户启用

net user 用户名 /active:no 指定用户禁用

net user 用户名 密码 /add 添加luoyu用户

net user 用户名 /del 删除luoyu用户

net user 用户名 新密码 更改密码

net user luoyu ""  指定用户名密码为空

net localgroup jishubu nihao /add    

net localgroup administrators nihao /add 把指定用户添加到指定组

net localgroup administrators nihao /del  把指定用户从指定组删除

net localgroup administrators /del 把指定组删除

netdom renamecomputer localhost /newname:"新名字"

net localgroup 查看组

net localgroup  shujubu  查看组的信息

gpsecpol /force 强制刷新策略