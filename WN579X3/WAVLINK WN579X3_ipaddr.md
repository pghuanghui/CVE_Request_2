## 0x01 Vulnerability description

an issue was discovered on WAVLINK WN579 X3 devices,Firmware package version M79X3.V5030.201201. The login.cgi does not filter the parameter keys, resulting in command injection in the page/login.shtml.

## 0x02 Affected version

```
WAVLINK WN579 X3 
```

## 0x03 Vulnerability

The value of v7 through the POST packet is ipaddr, and then v100 is equal to v7,use the system function directly to execute the v100 content，Use "xxx;command" for command injection

![image-20220907141811128](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_ipaddr.assets/image-20220907141811128.png)

![image-20220907141728802](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_ipaddr.assets/image-20220907141728802.png)

## 0x04 PoC verification

![image-20220907163845178](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_ipaddr.assets/image-20220907163845178.png)

## 0x05 Acknowledgement

PeiWen.Huang