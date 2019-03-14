# Ubuntu 16.04/18.04 重置登录密码

## 1 进入Recovery Mode

Recovery Mode即恢复模式, 在Grub启动菜单选择“Advanced Options for Ubuntu”, 如下图所示：

<div align="center">
<img src="./resource/figure/grub.png" height=30% width=60% >
</div>


## 2 选择 root Drop to root shell prompt

进入恢复菜单选择 root  Droop to root shell prompt, 然后回车

<div align="center">
<img src="./resource/figure/recover.png" height=30% width=60% >
</div>


## 3 依次执行如下命令

\# mount -o rw,remount /
\# ls /home      # 系统中的用户

\# passwd NEW_PASSWORD #重置密码

<div align="center">
<img src="./resource/figure/new_passwd.png" height=30% width=60% >
</div>


## 4 退出恢复模型，正常启动

输入exit命令回启动菜单，选择resume, 正常启动系统，在登录界面输入刚才新设的密码即可
