![License](https://img.shields.io/badge/license-GNU-green.svg?style=flat-square)

# **Salsa Tools - ShellReverse**
# **TCP/UDP/ICMP/ DNS and AV bypass, AMSI patched**

```
   _____       __              ______            __    
  / ___/____ _/ /________ _   /_  __/___  ____  / /____
  \__ \/ __ `/ / ___/ __ `/    / / / __ \/ __ \/ / ___/
 ___/ / /_/ / (__  ) /_/ /    / / / /_/ / /_/ / (__  ) 
/____/\__,_/_/____/\__,_/    /_/  \____/\____/_/____/  
                                                       

 [+] Starting the fucking Salsa...
 [+] EncrypterAssembly (Software to encrypt our payload)
 [+] EvilSalsa (This is our payload)
 [+] SalseoLoader (Software that we will use to load our encrypted payload)
```
Salsa Toos is a set of tools written in C # that allows you to have a shellreverse in any windows environment without needing powershell for its execution.


```
  ______                             _            
 |  ____|                           | |           
 | |__   _ __   ___ _ __ _   _ _ __ | |_ ___ _ __ 
 |  __| | '_ \ / __| '__| | | | '_ \| __/ _ \ '__|
 | |____| | | | (__| |  | |_| | |_) | ||  __/ |   
 |______|_| |_|\___|_|   \__, | .__/ \__\___|_|   
     /\                   __/ | || |   | |        
    /  \   ___ ___  ___ _|___/|_|| |__ | |_   _   
   / /\ \ / __/ __|/ _ \ '_ ` _ \| '_ \| | | | |  
  / ____ \\__ \__ \  __/ | | | | | |_) | | |_| |  
 /_/    \_\___/___/\___|_| |_| |_|_.__/|_|\__, |  
                                           __/ |  
                                          |___/   
			  
 [+] Software that encrypts the payload using RC4
 [+] We have the version in python and the version in .exe
```
# Usage EncrypterAssembly in python

```
python encrypterassembly.py <FILE> <PASSWORD> <OUTPUT>
```

# Usage EncrypterAssembly in .EXE

```
Encrypterassembly.exe <FILE> <PASSWORD> <OUTPUT>
```
![](https://github.com/Hackplayers/Salsa-tools/blob/master/images/encrypterpython.png)

```
   ___ __ __  ____  _            
  /  _]  |  ||    || |           
 /  [_|  |  | |  | | |           
|    _]  |  | |  | | |___        
|   [_|  :  | |  | |     |       
|     |\   /  |  | |     |       
|_____| \_/  |____||_____|       
                                 
  _____  ____  _     _____  ____ 
 / ___/ /    || |   / ___/ /    |
(   \_ |  o  || |  (   \_ |  o  |
 \__  ||     || |___\__  ||     |
 /  \ ||  _  ||     /  \ ||  _  |
 \    ||  |  ||     \    ||  |  |
  \___||__|__||_____|\___||__|__|
                                 
```
# Description

EvilSalsa is our payload. Basically what we do is load the System.Management.Automation .dll. Create a runspace and within that runspaces we have four types of shells (TCP / UDP / ICMP / DNS). When the EvilSalsa is loaded into the system, the first thing it does is to check if "c: \ windows \ system32 \ amsi.dll" is found in the system. If it is in the system, it is patched: D. Patching is a patch variant of CyberArk and Rastamouse.

AMSI Bypass Redux | CyberArk
https://www.cyberark.com/threat-research-blog/amsi-bypass-redux/
AMSI Bypass Rastamouse
https://rastamouse.me/2018/11/amsiscanbuffer-bypass---part-3/


