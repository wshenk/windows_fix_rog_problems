# How to fix problems with ASUS ROG Laptops running Windows  
Screen doesn't turn on correctly? Disable Fast Boot/Hibernation
Run CMD as an Administrator
```
powercfg.exe /h off
```

No power options available?
Run CMD as Administrator
```
reg query HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer
reg add HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer /v NoClose /t REG_DWORD /d 0
```
