## 「 关于DC1固件生成、刷写工具 」

此工具用于DC1固件的生成与刷写，请先接好线、配置好工具环境。

- 项目的整体情况，请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome)
- 配置文件下载，请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome/tree/master/yaml)
- TTL刷固件的接线及进入刷写模式方法请[参考文档内的说明](https://github.com/Samuel-0-0/phicomm_dc1-esphome/blob/master/cookbook)。


## Windows 系统搭建编译环境

**因platformio需要python2.7的环境，所以python2.7为必须。**

1. 下载 [git安装包-64位](https://github.com/git-for-windows/git/releases/download/v2.21.0.windows.1/PortableGit-2.21.0-64-bit.7z.exe) / [git安装包-32位](https://github.com/git-for-windows/git/releases/download/v2.21.0.windows.1/PortableGit-2.21.0-32-bit.7z.exe)
2. 下载 [python2.7安装包-64位](https://www.python.org/ftp/python/2.7.16/python-2.7.16.amd64.msi) / [python2.7安装包-32位](https://www.python.org/ftp/python/2.7.16/python-2.7.16.msi)
3. 下载（右键另存为） [DC1刷机工具（自搭环境版）](https://github.com/Samuel-0-0/esphome-tools-dc1/archive/lite.zip) 并解压
4. 解压Git安装包内所有文件到DC1刷机工具的Prerequisites\git里面，如下图

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/lite/Prerequisites/%E6%AD%A5%E9%AA%A44.png?raw=true)

5. 安装python到指定位置，如下图

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/lite/Prerequisites/%E6%AD%A5%E9%AA%A45.1.png?raw=true)

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/lite/Prerequisites/%E6%AD%A5%E9%AA%A45.2.png?raw=true)

6. 运行DC1工具箱，选择(3)升级编译环境，等待完成。

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/lite/%E5%B7%A5%E5%85%B7%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE.png?raw=true)

7. 将固件配置文件存放于DC1刷机工具的config_yaml目录内。
8. 执行菜单(1)编译DC1固件，确认无报错后执行菜单(2)升级DC1固件。注意！初次使用*必须*用TTL线刷，之后可以通过OTA升级。

### ==建议定期更新刷机工具==

# 错误解决
遇到未知错误，请删除config_yaml文件夹内.esphome和build下与配置文件对应的文件和文件夹！

如下图的错误：

![image](https://github.com/Samuel-0-0/esphome-tools-dc1/blob/lite/%E7%BC%96%E8%AF%91%E9%94%99%E8%AF%AF%E8%AF%B4%E6%98%8E.png?raw=true)
