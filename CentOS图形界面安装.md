## 图形界面安装 

**yum命令安装图形界面** 

```
yum groupinstall "X Window System" 
```

**安装GNOME桌面环境** 

```
yum groupinstall "GNOME Desktop Environment" 
```

**安装KDE桌面环境（KDE和GNOME任选其一都行）** 

```
yum groupinstall "KDE (K Desktop Environment)" 
```



## 图形界面切换 

**查看系统运行模式** 

```
systemctl get-default 
```

**设置系统启动后进入文本界面：** 

```
systemctl set-default multi-user.target 
```



**设置系统启动后进入图形界面：** 

```
systemctl set-default graphical.target 
```

**重启系统：** 

```
systemctl reboot 
```

**以文本界面启动后，执行以下命令启动图形界面：** 

```
startx 
```

Ctrl + Alt + F6 切换到文本界面（F1~F6都是文本界面，默认在F6） 

Ctrl + Alt + F7 切换到图形界面（F7~F12都是图形界面，默认在F7） 

Ctrl + Alt + backspace 重启当前图形界面
