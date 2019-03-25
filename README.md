# 「 DC1固件生成、刷写工具箱 」

此工具用于DC1固件的生成与刷写，请将固件配置文件存放于config_yaml
目录内。按照自己的情况修改配置文件中substitutions下面的参数。
然后执行菜单(1)，确认无报错后执行菜单(3)。

初次使用必须TTL线刷，后续可以通过OTA升级。
菜单(3)升级DC1固件 支持TTL和OTA双模式选择。


配置文件下载、TTL刷固件的接线及进入刷写模式方法请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome/blob/master/README.md)。

# 工具下载地址

直接右上角「 Clone or download 」  →  「 Download  ZIP 」

# 错误解决
遇到未知错误，请删除config_yaml文件夹内.esphome和build下与配置文件对应的文件和文件夹！

如下图的错误：
![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/master/%E7%BC%96%E8%AF%91%E9%94%99%E8%AF%AF%E8%AF%B4%E6%98%8E.png?raw=true)