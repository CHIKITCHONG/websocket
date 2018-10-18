# websocket
websocket聊天室


![demo](https://github.com/CHIKITCHONG/websocket/blob/master/demo.gif)

# 功能介绍
这是一个使用websocket、flask搭建的聊天室,可以聊天,加入房间,退出房间, 广播信息。

# 如何部署使用？
### 1.下载vagrant虚拟机. [链接](https://www.vagrantup.com/downloads.html)
### 2.下载vagrant镜像文件,建议使用：ubuntu/trusty64. [链接](https://app.vagrantup.com/boxes/search)
### 3.windows系统 需要在 bios 中开启 vt-x / amd-v,windows 10 需要禁用 hyper-v。
### 4.cd到项目根目录,将镜像文件放在项目根目录下,运行：
```
vagrant up
```
### 5.进行执行虚拟机的初始化（重新部署）,完成后进入虚拟机：
```
vagrant provision

### 登陆虚拟机
vagrant ssh
```
### 6.运行`app.py`启动项目：
```
# 查看虚拟机ip地址：
hostname -I

# 运行项目：
sudo python3 chat.py
```

#### 说明：由于socketio有bug,不支持window，所以需要在虚拟环境下运行
