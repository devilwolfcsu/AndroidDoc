# WifiConfiguration

public class WifiConfiguration extends Object implements Parcelable

[TOC]


## Summary

### 内部类

|类型|类名|描述|
|:--|:--|:--|
|class|WifiConfiguration.AuthAlgorithm|公认的IEEE802.11认证算法|
|class|WifiConfiguration.GroupCipher|公认的组密钥|
|class|WifiConfiguration.KeyMgmt|公认密钥管理方案|
|class|WifiConfiguration.PairwiseCipher|公认的WPA对称密钥|
|class|WifiConfiguration.Protocol|公认安全协议|
|class|WifiConfiguration.Status|网络配置的可能状态|

### 属性字段

|类型|字段|描述|
|:--|:--|:--|
|public String|BSSID|如果设置，则条目仅与指定BSSID相应的AP关联|
|public String|FQDN|一个控制节点（passpoint）完全限定域名|
|public String|SSID|网络SSID|
|public BitSet|allowedAuthAlgorithms|该配置支持的认证协议集合|
|public BitSet|allowedGroupCiphers|该配置支持的组密钥集合|
|public BitSet|allowedKeyManagement|该配置支持的密钥关系协议集合|
|public BitSet|allowedPairwiseCiphers|该配置支持的WPA对称密钥集合|
|public BitSet|allowedProtocol|该配置支持的安全协议|
|public WifiEnterpriseConfig|enterpriseConfig|关于配置指定的EAP方法、认证和连接设置等信息|
|public boolean|hiddenSSID|不广播SSID的网络，所以搜索需要使用特定SSID指针|
|public int|networkId|请求者使用的id,用于标识网络配置信息|
|public String|preSharedKey|WPA-PSK使用的预分享密钥|
|public int|priority|优先级，wpa_supplicant用来决策连接的AP|
|public String|providerFridenlyName|控制点信用提供者名称|
|public long[]|roamingConsortiumIds|漫游ID列表？？|
|public int|status|该网络配置信息的当权状态|
|public String[]|wepKeys|四个WEP密钥|
|public int|wepTxKeyIndex|默认的WEP密钥序列 0-3|

### 公共方法

|返回值|方法名|描述|
|:--|:--|:--|
|boolean|isPasspoint()|确定该配置是否是passpoint网络|
|String|toString()||
