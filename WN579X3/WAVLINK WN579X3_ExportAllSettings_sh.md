## 0x01 Vulnerability description

A vulnerability is in the 'extender_set_ssid.shtml' page of the WAVLINK WN579 X3,Firmware package version M79X3.V5030.201201

## 0x02 Affected version

```
WAVLINK WN579 X3
```

## 0x03 Vulnerability

Wavlink WN579X3 M79X3.V5030.201201 was discovered to contain a hardcoded encryption/decryption key for its configuration files at /etc_ro/lighttpd/www/cgi-bin/ExportAllSettings.sh.

When judging whether the user is valid, it will trigger the system to execute the command.

![image-20220907145803869](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_ExportAllSettings_sh.assets/image-20220907145803869.png)

The key is hardcoded and stored under /sbin/ExportAllSettings.sh

## 0x04 PoC verification

![image-20220907150216887](https://github.com/pghuanghui/CVE_Request_2/raw/main/WN579X3/WAVLINK%20WN579X3_ExportAllSettings_sh.assets/image-20220907150216887.png)

## 0x05 Acknowledgement

PeiWen.Huang