<a href="#"><img src="https://img.shields.io/github/forks/yuk1c/antiddos"/></a>
<a href="#"><img src="https://img.shields.io/github/license/yuk1c/antiddos"/></a>
<a href="#"><img src="https://img.shields.io/github/last-commit/yuk1c/antiddos"/></a>
<a href="#"><img src="https://img.shields.io/github/contributors/yuk1c/antiddos"/></a>
[![DeepSource](https://deepsource.io/gh/yuk1c/antiddos.svg/?label=active+issues&show_trend=true&token=tVgsBqvfV3KBAOkyv3rCEYiV)](https://deepsource.io/gh/yuk1c/antiddos/?ref=repository-badge)
### Fresh script for DDoS Mitigation using iptables and Kernel tweaks
This bash script adds rules to iptables, that protects you from Attacks on L4 OSI Model, like SYN Flood. Also, applies kernel tweaks. Working only on Debian-based.
##### If you are under volumetric DDoS - this rules doesn't help to you, bc this attacks overwhelm network capacity of ur server. Use VPS/VDS/DS with AntiDDoS.

### ⚙️ Installation:
```
git clone https://github.com/yuk1c/antiddos && cd antiddos && sudo bash antiddos-yuki && cd ..
```

### ⚔️ He give you protection against:

* TCP Flood attacks

* Fraggle attacks

* Spoofed attacks

* Attacks, that using invalid packets

* ICMP attacks

* UDP attacks

##### I remind you, that this script doesnt protect against Volumetric DDoS Attacks


### ❓️ Want to drop all ICMP?
```
sudo bash drop-icmp
```

I recommend you use drop-icmp script only if u under ICMP attack, or u want to make your server invisible for ICMP.

### 🔄 You can update this script, using:
```
sudo iptables -F; cd ~/antiddos && git pull && sudo bash antiddos-yuki
```

### ❌️ For deleting all rules and this script, write:
```
rm -fr ~/antiddos; sudo iptables -F
```
Delete parameters from /etc/sysctl.conf manually (if u need)


#### /etc/sysctl.conf tweaks not work on your system - use script named sysctl-tweaks. Execute as root, and add him to cron (because sysctl -w changes resets after reboot)

### If you want to support me:

#### Bitcoin
bc1qvuef0mzerxcv5t43puagtkw83ymjghuv6czkr5

#### Ethereum
0x33A109Ae4B7d77A105968Fb0aE6A9d69cd723Ed2

#### TON
EQARZzTYKAbo9GHS3jjTim-Hh2QLuTuCc3ilagv0YNTs-y5C


#### Thanks you for support 💙
