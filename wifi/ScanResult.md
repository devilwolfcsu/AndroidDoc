# ScanResult

public class ScanResult extends Object implements Parcelable

[TOC]

描述检测到的可访问点信息。除当前文档描述的属性外，请求者同时还跟踪quality、noise和maxbitrate属性，不过目前不对外部客户发布。

## Summary

### 常量

|类型|字段|描述|
|:--|:--|:--|
|int|CHANNEL_WIDTH_160MHZ|AP信道带宽为160MHZ|
|int|CHANNEL_WIDTH_20MHZ|AP信道带宽为20MHZ|
|int|CHANNEL_WIDTH_40MHZ|AP信道带宽为40MHZ|
|int|CHANNEL_WIDTH_80MHZ|AP信道带宽为80MHZ|
|int|CHANNEL_WIDTH_80MHZ_PLUS_MHZ|AP信道带宽为160MHZ，但是是80MHZ+80MHZ|

### 属性字段

|类型|字段|描述|
|:--|:--|:--|
|public string|BSSID|Ap地址|
|public string|SSID|网络名字|
|public string|capabilities|描述认证、密钥管理和接入点支持的加密方案|
|public int|centerfreq0|如果AP带宽为20MHZ则无用，如果是40、80或160MHZ，则表示为中心频率（MHZ），如果AP使用80+80MHZ，则为第一个频段的中心频率（MHZ）|
|public int|centerFreq1|仅用于80+80MHZ信道，如果是80+80MHZ，则表示第二个频段的中心频率（MHZ）|
|public int|channelWidth|AP信道带宽：见常量定义|
|public int|frequency|20MHZ频段信道下客户端通信的频率（MHZ）|
|public int|level|被检测到的信号强度（dBm,也被称为RSSI）|
|public CharSequence|operatorFriendlyName|表示AP发布的控制点操作名？？|
|public long|timestamp|时间戳（微秒）自启动到该Result被检测到？？|
|public CharSequence|venueName|表明AP发布的地点名，仅在控制网络且AP发布情况下有效|

### 共有方法

|返回类型|方法名|描述|
|:--|:--|:--|
|boolean|is80211mcResponder()||
|boolean|isPasspointNetwork()||
|String|toString()||
