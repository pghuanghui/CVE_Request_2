## 0x01 Vulnerability description

an issue was discovered on WAVLINK WN579 X3 devices,Firmware package version M79X3.V5030.201201. The login.cgi does not filter the parameter keys, resulting in command injection in the page/wifi_base.shtml.

## 0x02 Affected version

```
WAVLINK WN579 X3 
```

## 0x03 Vulnerability

Get the pingIp parameter through the POST packet and assign it to v2,use the fprintf function directly to execute the v2 content，Use "xxx;command" for command injection.

![image-20220907114543977](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_pingIp.assets/image-20220907114543977.png)

![image-20220907115933811](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_pingIp.assets/image-20220907115933811.png)

## 0x04 PoC verification

![image-20220907115321971](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_pingIp.assets/image-20220907115321971.png)

![image-20220907115344870](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_pingIp.assets/image-20220907115344870.png)

## 0x05 Acknowledgement

PeiWen.Huang