## 「 关于DC1固件生成、刷写工具 」

此工具用于DC1固件的生成与刷写，请先接好线并将固件配置文件存放于config_yaml目录内。

- 配置文件下载地址、系统的接入方法请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome)
- TTL刷固件的接线及进入刷写模式方法请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome/blob/master/cookbook/README.md)。

按照自己的情况修改配置文件中substitutions内的参数。

```
#--------------------- 只需要改这下面的内容 ---------------------
substitutions:
  #WiFi模组版本，型号中带B的为csm64f02_b，不带B的为csm64f02
  board_model: csm64f02_b
  #设备名称(多个dc1改成不一样的)
  device_name: phicomm_dc1
  #WiFi_SSID名称
  wifi_ssid: 'SSID'
  #WiFi密码
  wifi_password: '12345678'
  #OTA密码
  ota_password: '123456'
#--------------------- 只需要改这上面的内容 ---------------------
```
1. 关于WiFi模组版本的选择，请查看下图，找出自己对应的芯片版本即可。
看红色箭头的位置，带B的为csm64f02_b，不带B的为csm64f02

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/master/%E6%A8%A1%E7%BB%84%E5%9E%8B%E5%8F%B7%E9%80%89%E6%8B%A9.jpg?raw=true)

2. 以上步骤都完成后，打开工具，执行菜单：(1)编译固件，确认无报错后执行菜单：(3)升级DC1固件。

> 初次使用必须TTL线刷，后续可以通过OTA升级。
> 菜单(3)升级DC1固件 支持TTL和OTA双模式选择。

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/master/%E5%B7%A5%E5%85%B7%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE.jpg?raw=true)


## 工具下载地址

右上角「 Clone or download 」  →  「 Download  ZIP 」
### ==建议定期更新刷机工具==

# 错误解决
遇到未知错误，请删除config_yaml文件夹内.esphome和build下与配置文件对应的文件和文件夹！

如下图的错误：
![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/master/%E7%BC%96%E8%AF%91%E9%94%99%E8%AF%AF%E8%AF%B4%E6%98%8E.png?raw=true)