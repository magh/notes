# NetworkManager issues

## RTL8191SEvB not working with NM and Ubuntu/linux 3.5.0-18
	$ lspci -nn | grep 0280
	03:00.0 Network controller [0280]: Realtek Semiconductor Co., Ltd. RTL8191SEvB Wireless LAN Controller [10ec:8172] (rev 10)

### Reload module
*Didnt work*
	sudo modprobe -r rtl8192se
	sudo modprobe rtl8192se
	sudo rfkill unblock all
	sudo ifconfig wlan0 up

### rtl8192se_linux_2.6.0010.1012.2009.tar.gz
*Didnt work*
Download rtl8192se_linux_2.6.0010.1012.2009.tar.gz

Comment out IEEE80211_HW_BEACON_FILTER from base.c (line 319)
	sudo make && sudo make install

### Replace Network-manager
*Didnt work*
	sudo apt-get remove network-manager
	sudo apt-get install wicd

### Backport modules
*Seems to fix it*
	linux-backports-modules-cw-3.6-3.5.0-18-generic

### Using newer kernel
https://wiki.ubuntu.com/Kernel/MainlineBuilds?action=show&redirect=KernelMainlineBuilds

### Changes in /etc/protocols, /etc/services, rc.conf?
Downgrading initscripts to 2012.06.3-2 should work around it for now.

'network' and 'networkmanager' enabled in rc.conf DAEMONS.
Disable 'network' and leave only 'networkmanager'.

Reference link: https://bugs.archlinux.org/task/30892

### Reset wicd
	rc.d stop wicd
	rm /etc/wicd/*.conf
	rc.d start wicd

# Gateway
There should be only one default gw.

example:
```
# route
Kernel IP routing table
Destination     Gateway         Genmask         Flags Metric Ref    Use Iface
192.168.1.0     *               255.255.255.0   U     0      0        0 eth0
80.216.66.0     *               255.255.254.0   U     0      0        0 eth1
loopback        *               255.0.0.0       U     0      0        0 lo
default         ML-DOC-4-Cable6 0.0.0.0         UG    0      0        0 eth1
```
