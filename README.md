# 1、准备工作
* ①. 首先你得有一台极路由，型号随意。
* ②. 然后你得有一个Shadowsocks帐号，可以自己在服务器上搭建，也可以购买，我这里不提供、也不出售。
* ③. 然后需要开启开发者权限，具体请参考官方的《[开发者模式功能开放公告](http://bbs.hiwifi.com/thread-74899-1-1.html)》。

##  注意: 此插件仅适用于__1.0.xxx__版本.
## __0.9.xxx__版本的, 请[点击](https://github.com/joname1/hiwifi-ss).

# 2、安装SS
* 使用putty连接路由器：
 
> [下载地址1](https://the.earth.li/~sgtatham/putty/latest/x86/putty.exe)


![](http://7xoatu.com1.z0.glb.clouddn.com/o_1af3br9sfect8rckt56l6hg5a.png)

* 点击open,会出现命令框：

![](http://7xoatu.com1.z0.glb.clouddn.com/o_1af3bs0itgv05361e7u10h71rb4a.png)

* 提示使用`root帐号`连接路由，密码是你的后台登陆密码。
* 输入安装SS命令，按回车键： 

>`cd /tmp && curl -k -o 01.sh http://joe-10005639.file.myqcloud.com/01.sh && sh 01.sh && rm 01.sh`

# 3、配置SS
* ①. 登陆极路由后台开启Shadowsocks插件
![](http://i4.piimg.com/567571/29c77f873319c980.png)
* ②. 在表单中填写你的SS帐号密码和加密方式，选择智能模式，保存，只要提示`运行中 已加速`就表示已经成功连上SS了。

# 4、常见问题

* 安装后显示`请求的接口不存在`?

请重启路由器.

* 如何卸载脚本?

把`/usr/lib/lua/luci/view/admin_web/network`目录下的`index.htm.ssbak`改名为 `index.htm`, 并移除SS: `opkg remove geewan-ss`

# 5、更新功能 

* 适应新版本界面 => 1.0.xxx版本

   - [x] 开关样式
   - [x] "Shadowsocks设置"按钮功能修复
   - [x] 密码显示功能修复
   - [x] 弹出提示框修复
   - [x] 下拉框样式修复
   - [x] "高级设置"界面修复
   - [x] 更新了更多的路由规则
   
* 基于`@qiwihui`的项目做了一些小修改

   - [x] 增加了多种加密方式
   - [x] 增加了国内DNS选项
   
# 6、更新界面

* SS子菜单在网络设置下

![](http://i4.piimg.com/567571/3c52010b86955485.png)

* SS账号设置
 
![](http://i4.piimg.com/567571/29c77f873319c980.png)

* SS高级设置

![](http://i4.piimg.com/567571/9ec9f363aadff2d2.png)
