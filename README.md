# AdbCommand
收集adb常用的命令， 欢迎大家分享在工作中，常用的工作命令

---
**adb devices**
</br>
列举出当前连接的所有设备

---

**adb -s 序列号  install -r -t apk** </br>
主要想介绍一下， 如果adb devices列举了当前连接了多台设备，在通过adb 执行任何一个命令时，需要添加 -s参数 加上序列号。

---
