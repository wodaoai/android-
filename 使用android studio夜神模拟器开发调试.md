## 使用android studio夜神模拟器开发调试 ##

相信很多android开发者都会遇到这样的问题
1、需要不同分辨率的手机，成本好高啊
2、USB连接线不稳，总是容易断开，重新连接
那么，请使用夜神模拟器来辅助开发，高效、稳定。
intellij idea 及 eclipse也适用

###工具 ###
- android studio / intellij idea / eclipse
夜神模拟器
###操作步骤 ###
- 通过android studio新建自己的工程
- 下载并安装夜神模拟器，夜神模拟器官网下载[https://www.yeshen.com/](https://www.yeshen.com/ "")
- 先启动夜神模拟器
- 然后运行cmd命令，cd到夜神安装目录，执行命令
- **nox_adb.exe connect 127.0.0.1:62001**
- 连接到模拟器
###也可以把命令保存到.bat执行如下：###
切换盘符
d:                   
打开夜神模拟器安装目录
cd D:\Program Files (x86)\Nox\bin\
执行下面代码
nox_adb.exe connect 127.0.0.1:62001

pause
###注意事项###
- 如果无法看到夜神模拟器，请adb后，重新启动下夜神模拟器
- intellij idea eclipse同样适用





