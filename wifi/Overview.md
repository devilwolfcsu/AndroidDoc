# Overview

[TOC]

提供管理设备Wi-Fi功能的各种类
Wi-Fi APIs提供一个方式使得应用程序可以与低级别的无线层级通信，以此来提供Wi-Fi访问。几乎可以访问该设备提供的所有信息，包括连接网络的连接速度、IP地址、认证状态以及其他可访问的网络信息。另外一些API包括扫描、添加、保存、终止和启动Wi-Fi连接。

一些APIs可能需要一些用户权限：

* `ACCESS_WIFI_STATE`
* `CHANGE_WIFI_STATE`
* `CHANGE_WIFI_MULTICAST_STATE`

**NOTE:**并不是所有的安卓设备提供Wi-Fi功能，如果你的应用使用Wi-Fi,需要在manifest文件中使用`<uses-feature>`标签声明：

```  java
<manifest ...>
    <uses-feature android:name="android.hardware.wifi" />
    ...
</manifest>
```

## Classes

|类名|描述|
|:--|:--|
|ScanResult|描述检测到的可访问点的信息|
|WifiConfiguration|代表Wi-Fi网络配置的类，其中包括安全配置信息|
|WifiConfiguration.AuthAlgorithm|公认的IEEE 802.11认证算法|
|WifiConfiguration.GroupCipher|公认的组密钥|
|WifiConfiguration.KeyMgmt|公认的密钥管理方案|
|WifiConfiguration.PairwiseCipher|公认的WPA对称密码|
|WifiConfiguration.Protocol|公认的安全协议|
|WifiConfiguration.Status|网络配置的可能状态|
|WifiEnterpriseConfig|无线网络的企业配置信息|
|WifiEnterpriseConfig.Eap|所使用的可扩展身份验证协议方法（Extensible Authentication Protocol）|
|WifiEnterpriseConfig.Phase2|内部验证方法|
|WifiInfo|描述任何处于连接状态和正在连接状态的信息|
|WifiManager|提供Wi-Fi管理的主要API方法|
|WifiManager.MulticastLock|允许应用程序接受无限广播数据包|
|WifiManager.WifiLock|允许应用程序保持Wi-Fi无线电保持活动状态|
|WifiManager.WpsCallback|启动WPS时提供回调功能的接口|
|WpsInfo|表示Wi-Fi保护设置（Wi-Fi Protected Setup）|

## Enums

|枚举名|描述|
|:--|:--|
|SupplicantState|定义在defs.h中wpa_supplicatn|