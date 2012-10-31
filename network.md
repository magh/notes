# NetworkManager issues

## RTL8191SEvB not working with NM and Ubuntu/linux 3.5.0-18
	$ lspci -nn | grep 0280
	03:00.0 Network controller [0280]: Realtek Semiconductor Co., Ltd. RTL8191SEvB Wireless LAN Controller [10ec:8172] (rev 10)



# Gateway
There should be only one default gw.

example:
	# route
	Kernel IP routing table
	Destination     Gateway         Genmask         Flags Metric Ref    Use Iface
	192.168.1.0     *               255.255.255.0   U     0      0        0 eth0
	80.216.66.0     *               255.255.254.0   U     0      0        0 eth1
	loopback        *               255.0.0.0       U     0      0        0 lo
	default         ML-DOC-4-Cable6 0.0.0.0         UG    0      0        0 eth1
