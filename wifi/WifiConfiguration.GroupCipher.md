# WifiConfiguration.GroupCipher

public static class WifiConfiguration.GroupCipher extends Object

[TOC]

公认的组密钥

``` java
 CCMP = AES in Counter mode with CBC-MAC [RFC 3610, IEEE 802.11i/D7.0]
 TKIP = Temporal Key Integrity Protocol [IEEE 802.11i/D7.0]
 WEP104 = WEP (Wired Equivalent Privacy) with 104-bit key
 WEP40 = WEP (Wired Equivalent Privacy) with 40-bit key (original 802.11)
```

## Summary

### 常量

|类型|常量字段|描述|
|:--|:--|:--|
|int|CCMP|AES in Counter mode with CBC-MAC [RFC 3610, IEEE 802.11i/D7.0]|
|int|TKIP|Temporal Key Integrity Protocol [IEEE 802.11i/D7.0]临时密钥完整性协议|
|int|WEP104|WEP104 = WEP (Wired Equivalent Privacy) with 104-bit key|
|int|WEP40|WEP40 = WEP (Wired Equivalent Privacy) with 40-bit key (original 802.11)|
|String|varName||

### 字段

|类型|字段名|描述|
|:--|:--|:--|
|public static final String[]|strings||
