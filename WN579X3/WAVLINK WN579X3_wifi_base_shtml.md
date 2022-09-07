## 0x01 Vulnerability description

A vulnerability is in the 'extender_set_ssid.shtml' page of the WAVLINK WN579 X3,Firmware package version M79X3.V5030.201201

Unauthorized users can obtain the key information of the router by visiting:

```
http://xxx.xxx.xxx.xxx/wifi_base.shtml
```

## 0x02 Affected version

```
WAVLINK WN579 X3
```

## 0x03 Vulnerability

The interface can be accessed without authorization, and can operate WiFi at the same time.

![image-20220907105021547](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_wifi_base_shtml.assets/image-20220907105021547.png)

## 0x04 PoC verification

![image-20220907105112421](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_wifi_base_shtml.assets/image-20220907105112421.png)

## 0x05 Acknowledgement

PeiWen.Huang