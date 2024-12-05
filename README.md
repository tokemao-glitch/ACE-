![Logo](https://cdn.discordapp.com/attachments/1284099506459250762/1313887370642329611/image-removebg-preview_2.png?ex=6751c478&is=675072f8&hm=71b3a76dc7c28b2aab8e63f61a70e17c6a35d86d1988722fb5c3901496eb8076&)
# [A.C.E] (Access Control Expert) 🌌 

ACE is designed to perform security testing efficiently and discreetly. It automatically connects to the Tor network in the background, ensuring anonymity during operations. It includes an intuitive menu with specialized tools! - **ONLY FOR WINDOWS** (for now)

![LOCO](https://img.shields.io/github/stars/tokemao-glitch/tokemao) ![DOWNLOADS](https://img.shields.io/github/downloads/tokemao-glitch/tokemao/total?style=plastic) ![COMMITS](https://img.shields.io/github/commit-activity/w/tokemao-glitch/tokemao)
 
## Features 💻

- SQLi Advanced Scanners.
- Host research, ip and servers.
- DoS Attacks.
- Customizable injections.


## 🛠Windows compatible tools included in ACE:

 - [SQLiScan](https://github.com/hackyguru/SQLiScan) (A python based tool for finding SQL vulnerable sites.)
 - [ScanQLi](https://github.com/bambish/ScanQLi) (SQLi scanner to detect SQL vulns.)
 - [Nmap](https://nmap.org/) (Open source tool used for network scanning and mapping, identifying hosts, services, and vulnerabilities.)
 - [Slowloris](https://github.com/gkbrk/slowloris) (Low bandwidth DoS tool.)
 - [TOR](https://github.com/gkbrk/slowloris) (Routes traffic through distributed nodes to hide identity)
 - [XSSStrike](https://github.com/s0md3v/XSStrike) (Advanced XSS Scanner)
 - [DSSS](https://github.com/stamparm/DSSS) (<100 Lines of code SQLi Scanner)
 - [Dosinator](https://github.com/HalilDeniz/Dosinator) (powerful Denial of Service testing tool developed in Python)


## Install & Deploy ⚙

- Download this repository.

- Install the requirements:

```batch
  pip install -r requirements.txt
```
- Setup TOR proxy:
`1` - Download [TOR](https://www.torproject.org/dist/torbrowser/14.0.3/tor-browser-windows-x86_64-portable-14.0.3.exe)

`2` -  Go to **\AppData\Roaming\tor**

`3` - Edit **torcc** file, delete everything that is written and paste the following:
```
ControlPort 9051
SocksPort 9050
SocksPolicy accept 127.0.0.1
SocksPolicy reject *
HashedControlPassword 16:YOURHASHEDPASSWORD
```
(You need to set up your HashedControlPassword so that Tor can use the drivers that are used to change the IP in real time) See how [HERE](https://chatgpt.com/share/67507993-2c08-800c-be33-df7c264c1eea)

`4` - Open a terminal and run the script:
```bash
python main.py
```
## Supported OS (ONLY WINDOWS) 🖥
 I'm testing this script only on windows to start a stable compatibility with BlackArch, Kali Linux, Ubuntu x64 and Parrot, for now it only works **on windows**, but I'm working to port the script to other distributions. ❤
| OS            | Support                                                               |
| ----------------- | ------------------------------------------------------------------ |
| Windows | ✔ | 
| Kali Linux |❌|
| BlackArch | ❌ |
| Ubuntu | ❌ |
| Parrot | ❌ |