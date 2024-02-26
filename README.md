# Warp on Warp
[This Config file](Configs/WarpOnWarp-HiddifyNext.json) can be used directly in the [Hiddify Next](https://github.com/hiddify/hiddify-next/releases) App.

But it is better to make your personal config to have better speed and lower delay.

## How to make personal warp config?
### Windows
1. Copy the [Config file](Configs/WarpOnWarp-HiddifyNext.json) to an editor of your choice.
2. Download and extract [this zip file](https://github.com/soohrab/Warp-On-Warp/raw/main/WarpIP-PortScanner/WarpIP-PortScanner-Win-v23.11.15.zip)
3. Open the WarpIP-PortScanner.bat and select option 1 and press enter to start the scanner.
4. Replace the two IP/Ports of the copied config file (Step 1) with the best IP/Port from the result.csv of the step 3. (the one with the lowest ping)
5. Download and drag the windows version of [Warp-Reg](https://github.com/badafans/warp-reg/releases) to the terminal and press enter. (Run the instruction two times to acquire two free Warp accounts)
6. Each time you run it, writes 3 lines including IPv6, private key and reserved bytes. You can replace the corresponding values of the copied config (Step 1) with these values
### When pasting IPv6, be careful not to include '/128' and the end of the line in your selection.
---
### Android, Linux and Mac
1. Copy the [Config file](Configs/WarpOnWarp-HiddifyNext.json) to an editor.
2. Run the below command in the termux(Android Shell), linux or mac to acquire best working IP/Ports of the Cloudflare Warp.
```
bash <(curl -fsSL https://raw.githubusercontent.com/Ptechgithub/warp/main/endip/install.sh)
```
3. After running the command select option 1.
4. Replace the two IP/Ports of the copied config file (Step 1) with one of the resulted IP/Port of the step 2.
5. Run the below instruction two times to acquire two free Warp accounts. Each time you run it, writes 3 lines including IPv6, private key and reserved bytes. You can replace the corresponding values of the copied config (Step 1) with these values.
```
curl -sL "https://api.zeroteam.top/warp?format=sing-box" | grep -Eo --color=never '"2606:4700:[0-9a-f:]+/128"|"private_key":"[0-9a-zA-Z\/+]+="|"reserved":\[[0-9]+(,[0-9]+){2}\]'
```
---
 ## Now try the new config useing the Hiddify Next App.

 ### Credits [Yonggekkk](https://github.com/yonggekkk/warp-yg) for the windows warp IP scanner
