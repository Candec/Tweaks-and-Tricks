# Tweaks-and-Tricks

## 1.Windows
### 1.1 Regedit

*Remove Windows menu load delay - default 400ms*
1.HKEY_CURRENT_USER\Control Panel\Desktop
2.edit to "0" 

*Windows 10 context menu without "show more"*
1.HKEY_CURRENT_USER\SOFTWARE\CLASSES\CLSID
2.Create a new Folder with name "86ca1aa0-34aa-4e8b-a509-50c905bae2a2"
3.Create a new Key with name "InprocServer32"
4.Restart computer

or

1.Paste in execute: reg.exe add "HKEY_CURRENT_USER\SOFTWARE\CLASSES\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve