# Working wifi client config

## Infos
Works on Debian 10

## DHCP config
```
auto INTERFACE_NAME
iface INTERFACE_NAME inet dhcp
	wpa-ssid WIFI_SSID
	wpa-ap-scan 1
	wpa-scan-ssid 1
	wpa-key-mgmt WPA-PSK
	wpa-group CCMP TKIP
	wpa-proto RSN WPA
	wpa-psk WIFI_PASSWORD
```

## Static IP address config
```
auto INTERFACE_NAME
iface INTERFACE_NAME inet static
	wpa-ssid WIFI_SSID
	wpa-ap-scan 1
	wpa-scan-ssid 1
	wpa-key-mgmt WPA-PSK
	wpa-group CCMP TKIP
	wpa-proto RSN WPA
	wpa-psk WIFI_PASSWORD
	address 192.168.1.120
	netmask 255.255.255.0
	gateway 192.168.1.1
	dns-nameservers 8.8.8.8
```