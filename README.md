# btwild
宝塔又作妖辣


## 一键干掉宝塔的强制登录  
`rm -f /www/server/panel/data/bind.pl`  

## 关闭安全入口：  
`rm -f /www/server/panel/data/admin_path.pl`  

## 修改面板密码，如要改成123456  
`cd /www/server/panel && python tools.py panel 123456`  

## 修改面板端口，如要改成8881  
`echo '8881' > /www/server/panel/data/port.pl && /etc/init.d/bt restart`  

## 快速降级  
```
wget http://download.bt.cn/install/update/LinuxPanel-7.7.0.zip
unzip LinuxPanel-*
cd panel
bash update.sh
cd .. && rm -f LinuxPanel-*.zip && rm -rf panel
 ```
