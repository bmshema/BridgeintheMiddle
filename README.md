# BridgeintheMiddle
This script automates the process of serving an evil twin AP from a remote bridging device and collecting traffic to view locally in Wireshark.

As is, this script is used with a Raspberry Pi with LTE modem connected over Wireguard VPN as the remote device and executed from your local machine.

## Dependencies:

### Local
```bash
sudo apt install wireshark sshpass
```

### Remote
```bash
sudo apt install haveged hostapd git util-linux procps iproute2 iw dnsmasq iptables
```

```bash
git clone  https://github.com/oblique/create_ap.git 
cd create_ap
sudo make install
```

create_ap is used because it just works better than any tool actually meant for man-in-the-middle applications.

![image](https://github.com/bmshema/BridgeintheMiddle/assets/92175742/dc0a57f8-28db-4e5b-a6da-2b75e729ccbf)

