# [OpenPuya](https://www.py32.org/)

为了弥补官方网站的资料更新不及时，我们将作为一个非官方的资料库，收集普冉半导体公司的产品资料。

# 版权声明
本组织下的所有资料均来自于普冉半导体公司官方，版权归普冉半导体公司所有。本组织下的所有资料仅供学习交流使用，本组织不对资料的准确性和完整性做任何保证，亦不承担任何法律责任。如有侵权，请联系我们删除。

## JFlash 插件

https://www.py32.org/tool/PY32_JFlash_Plugin.html

## 使用方法

### V7.62 以上的版本

V7.62 以上的 J-Link 版本对设备描述的 xml 进行了解耦，为了使 J-Link 软件能够识别新设备，需要将先前创建的 XML 文件放在中央 JLinkDevices 文件夹中。

我们可以在以下路径找到：

| 操作系统 |                         路径                          |
| :------: | :---------------------------------------------------: |
| Windows  |  C:\Users\<USER>\AppData\Roaming\SEGGER\JLinkDevices  |
|  MacOS   | $HOME/Library/Application Support/SEGGER/JLinkDevices |
|  Linux   |           $HOME/.config/SEGGER/JLinkDevices           |

如果没有找到`JLinkDevices`文件夹，可以手动创建一个。

打开该文件夹之后，将`Devices/Puya`文件夹复制过去即可。

### V7.62 以下的版本

V7.62 以下的版本，需要自行拼接设备的 xml，我们打开安装的`J-Link`的安装目录，找到`JLinkDevices.xml`文件，将此仓库下的`all.xml`文件中的内容复制插入到`JLinkDevices.xml`文件中最后的`</Database>`标签前。然后将`Device` 文件夹复制到`J-Link`的安装目录下。
