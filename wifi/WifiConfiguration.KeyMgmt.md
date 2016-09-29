# WifiConfiguration.KeyMgmt

public static class WifiConfiguration.KeyMgmt extends Object

[TOC]

公认的密钥管理机制

## Summary

### 常量

|类型|常量名|描述|
|:--|:--|:--|
|int|IEEE8021x|IEEE 802.1X使用EAP认证和动态生成WEP密钥方式（可选）|
|int|NONE|未使用WPA；明文或者静态WEP|
|int|WPA_EAP|WPA使用EAP认证|
|int|WPA_PSK|WPA预分享密钥（需要指定preSharedKey）|
|String|varName||

### 属性变量

|类型|变量名|描述|
|:--|:--|:--|
|public static final String[]|strings||
