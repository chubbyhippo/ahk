## Usage

```
Use Capslock to change between languages (Shift + Alt)
Use Shift + Capslock to Capslock
```
```
$WebClient=New-Object Net.WebClient
$Uri='https://raw.githubusercontent.com/chubbyhippo/ahk/master/CapsToChangeInputLanguage.ahk'
$WebClient.DownloadFile($Uri, "$Home\CapsToChangeInputLanguage.ahk")
$WshShell = New-Object -comObject WScript.Shell
$Shortcut = $WshShell.CreateShortcut("$Home\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\CapsToChangeInputLanguage.lnk")
$Shortcut.TargetPath = "$Home\CapsToChangeInputLanguage.ahk"
$Shortcut.Save()
```
