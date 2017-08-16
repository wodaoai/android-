##android结束占用adb命令.bat##

## 将下面命令行保存到.bat文件双击运行 ##
@echo off
color a  
title ReleaseAdbPort  
echo ---------------------------  
echo Checking adb port...  
for /F "usebackq tokens=5" %%a in (`"netstat -ano |   findstr "5037""`) do (  
if not "%%a" =="0" call :ReleasePort %%a
)  
echo ---------------------------  
echo adb port has been released!  
echo ---------------------------  
pause  

exit  

:ReleasePort  
TASKKILL /f /PID %1  


