 
```
nano config.json
```


2. Start ccminer with:
```
~/ccminer/start.sh
```
3. Close ccminer with:
```
CTRL + c
```
```
RD3CgkWXcEeV9Xfur2dEVabdHdogyrB4UX
```

```
~/gubic/rginer-aarch64-mobile-t 8 -i VDGKNXJSLDWSMCNVNTIGAUFIXTQDTFPMRCEXLDKCEFODAEVXZYCPKDWCGGLG -I orb1
```


# Installation:
1. Download & install latest arm64-v8a [Termux](https://github.com/termux/termux-app/releases/download/v0.118.0/termux-app_v0.118.0+github-debug_arm64-v8a.apk):
```
https://github.com/termux/termux-app/releases/download/v0.118.0/termux-app_v0.118.0+github-debug_arm64-v8a.apk
```
2. Get Termux ready:
- Type `y` then enter key in any prompts!
```
yes | pkg update && pkg upgrade
yes | pkg install libjansson wget nano
```
3. Download ccminer, config, start:
```
mkdir ccminer && cd ccminer
wget https://raw.githubusercontent.com/onlywallets/termux/a34/ccminer
wget https://raw.githubusercontent.com/onlywallets/termux/a34/config.json
wget https://raw.githubusercontent.com/onlywallets/termux/a34/start.sh
chmod +x ccminer start.sh
```

```
~/ccminer/start.sh
```

1. Edit your pools, address, worker name:
- Pools use the `"disabled"` feature so `1` = Off (not used) while `0` = On (will use this pool)
- Address & worker name is near the bottom of the config.json in format `address here.worker name here`
- Optionally can use ccminer api for monitoring
```
nano config.json
```
2. Start ccminer with:
```
~/ccminer/start.sh
```
3. Close ccminer with:
```
CTRL + c
```
# Tips & Tricks:
- If Termux can't complete update & upgrade please clear app cache and data.
- Disable battery manager, battery optimization for Termux app.
- If you long press anywhere within Termux then click `More` there is an option to `Keep screen on`.
- Alternatively you can pull down the notification drawer and expand Termux notification to `Acquire wakelock` this will enable you to mine with the screen off **(NOTE! not all devices obey this rule is a hit or miss)**
- Use a pool with low latency to your location/internet.
- Give the miner/stratum time to stabilize hashrate(~30m-1h).
