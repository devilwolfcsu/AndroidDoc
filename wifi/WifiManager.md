# WifiManager
  public class WifiManager
  extends Object

  java.lang.Object
     android.net.WifiManager

[TOC]

该类提供管理Wifi连接相关的主要API，可以通过如下方法获得一个实例：Context.getSystemService(Context.WIFI_SERVICE)。它主要处理以下几个功能：

* 网络配置列表。这个列表可以被访问、更新并且其中每个列表项中的属性可被修改；
* 当前处于激活状态的Wi-Fi网络，如果有连接。连接可以被建立和关闭，并且可以获取该网络的动态信息；
* 返回访问热点扫描结果，包含足够的信息来判断连接那个访问点；
* 定义任何类型的Wi-Fi状态变化的各种传播意向动作的名称。

## 概述

### 内置类
|类型|类名|描述|
|:--|:--|:--|
|class|WifiManager.MulticastLock|允许一个应用接受wifi 广播包|
|class|WifiManager.WifiLock|允许一个应用保持Wifi醒来|
|class|WifiManager.WpsCallback|为启动WPS动作踢动回调接口|

### 常量
|类型|命名|描述|
|:--|:--|:--|
|String|`ACTION_PICK_WIFI_NETWORK`|操作：选择一个Wi-Fi网络连接|
|String|`ACTION_REQUEST_SCAN_ALWAYS_AVAILABLE`|活动操作：显示系统活动，允许用户启动扫描甚至关闭网络|
|int|`ERROR_AUTHENTICATING`|如果出现认证问题，返回该错误码|
|String|`EXTRA_BSSID`|给定BSSID字符串，用于连接网络|
|String|`EXTRA_NETWORK_INFO`|用于查找已连接网络NetworkInfo对象的查找Key|
|String|`EXTRA_NEW_RSSI`|给定RSSI请求int值用于查找的key|
|String|`EXTRA_NEW_STATE`|查找SupplicantState对象的Key|
|String|`EXTRA_PREVIOUS_WIFI_STATE`|之前的网络状态|
|String|`EXTRA_RESULTS_UPDATED`||
|String|`EXTRA_SUPPLICANT_CONNECTED`||
|String|`EXTRA_SUPPLICANT_ERROR`||
|String|`EXTRA_WIFI_INFO`||
||||

### 公共方法
|返回类型|方法定义|描述|
|:--|:--|:--|
|int|addNetwork(WifiConfiguration config)|向配置网络集合中添加一个新的网络描述|
|static int|calculateSignalLevel(int rssi,int numLevels)|计算信号级别|
|void|cancelWps(WifiManager.WpsCallback listener)|取消任何正在进行的Wi-Fi保护设置|
|static int|compareSignalLevel(int rssiA,int rssiB)|比较两个信号的强度|
|WifiManager.MulticastLock|createMulticastLock(String tag)|创建一个新MulticastLock实例|
|WifiManager.WifiLock|createWifiLock(String tag)|创建一个新WifiLock实例|
|WifiManager.Wifi|createWifiLock(int lockType,String tag)|创建一个新WifiLock实例|
|boolean|disableNetwork(int netId)|使一个配置网络失效|
|boolean|disconnect()|与当前激活的连接点断开|
|boolean|enableNetwork(int netId,boolean disableOthers)|允许之前的配置网络连接|
|List`<WifiConfiguration>`|getConfiguredNetworks()|返回配置的所有网络列表|
|int|getWifiState()|获取Wi-Fi是否可用状态|
|boolean|is%gHzBandSupported()||
|boolean|isDeviceToApRttSupported()||
|boolean|isEnhancedPowerReportingSupported()||
|boolean|isP2PSupport()||
|boolean|isPreferredNetworkOffloadSupported()||
|boolean|isScanAlwaysAvailable()|检查扫描是否一直可用|
|boolean|isTdlsSupported()||
|boolean|isWifiEnabled()|返回Wi-Fi是可用还是不可用|
|boolean|pingSupplicant()|检查请求守护程序是否相应请求|
|boolean|reassociate()|重新连接当前访问热点，即使我们已经连接|
|boolean|reconnect()|如果当前无连接，连接当前激活热点|
|boolean|removeNetwork(int netId)|从配置网络列表中剔除制定网络配置|
|boolean|saveConfiguration()|告诉请求者（supplicant）持久化当前配置网络|
|void|setTdlsEnabled(InetAddress remoteIpAddress,boolean enable)|开启/取消TDLS在特定的本地路由|
|void|setTdlsEnableWithMacAddress(String remoteMacAddress,boolean enable)|与setTdlsEnabled相似，允许指定MAC地址|
|boolean|setWifiEnabled(boolean enabled)|启用或关闭Wi-Fi|
|boolean|startScan()|扫描可访问节点|
|void|startWps(WpsInfo config,WifiManager.WpsCallback listener)|开始Wi-Fi保护|
|int|updateNetwork(WifiConfiguration config)|对一个已经存在的网络配置更新网络配置|

### 保护方法
|返回类型|方法定义|描述|
|:--:|:--:|:--:|
|void|finalize()|垃圾回收器调用|
