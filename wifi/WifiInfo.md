# WifiInfo

public class WifiInfo extends Object implements Parcelable

[TOC]

描述连接的WiFi状态或正在连接的状态

## Summary

### 常量

|类型|常量名|描述|
|:--|:--|:--|
|String|FREQUENCY_UNITS|频率单位（MHZ）|
|String|LINK_SPEED_UNITS|连接速度单位（Mbps）|

### 共有方法

|返回值|方法名|描述|
|:--|:--|:--|
|String|getBSSID()|返回当前AP的basic service set identifier(BSSID)|
|static NetworkInfo.DetailedState|getDetailedStateOf(SupplicantState suppState)|将请求者状态转换成细粒度的网络连接状态|
|int|getFrequency()|返回当前频率|
|boolean|getHiddenSSID()||
|int|getIpAddress()||
|int|getLinkSpeed()|连接速度|
|String|getMacAddress()||
|int|getNetworkId|每一个网络配置有唯一的ID表示，由请求者使用，用来标识配置信息|
|int|getRssi|返回接受信号强度received signal strength indicator of the current 802.11|
|String|getSSID()|返回该802.11网络的service set identifier(SSID)|
|SupplicantState|getSupplicantState()|返回请求者详细状态信息|
|String|toString()||
