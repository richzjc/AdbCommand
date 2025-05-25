# AdbCommand
最近由Android手机应用开发，转行到了车载应用开发，主要是我现在负责车载Launcher,需要用到很多adb指令。
发现有很多adb指令，还不会使用，集思广益，
收集adb常用的命令， 欢迎大家分享在工作中，常用的工作命令， **感谢，感谢！！！**

[github地址](https://github.com/richzjc/AdbCommand/edit/main/README.md)
---
**adb devices**
</br>
列举出当前连接的所有设备

---

**adb -s 序列号  install -r -t apk** </br>
主要想介绍一下， 如果adb devices列举了当前连接了多台设备，在通过adb 执行任何一个命令时，需要添加 -s参数 加上序列号。

---

**adb root** </br>
以root模式运行adbd服务， 拥有最高权限，能够修改系统文件，尤其是从事内置应用开发， Launcher之类，经常会用到。比如/system目录

---

**adb remount** </br>
Android 系统开发和高级调试的核心工具，通过解除 /system 分区的只读限制，允许对系统进行深度修改，目前我是从事车载Launcher开发，经常会用到这个命令

---

**adb push file destinueDir** </br>
推送一个文件到系统指定目录，像推送一个apk到系统目录， 或者使用过frida的朋友都应该使用过这个命令

---

**adb logcat** </br>
查看系统的日志

**adb logcat -f file**</br>
将系统的日志保存到文件

---

**adb shell pidof 包名**</br>
获取某一个进程的进程id

---

**adb shell kill 进程id**</br>
杀掉一个进程

---

**adb shell**</br>
进入设备的linux环境

---

**adb uninstall 包名**</br>
卸载指定包名的应用

---
