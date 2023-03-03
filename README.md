# mcu-jlink-pack JLINK 的扩展包（一些暂时没有被 Segger 维护 JFlash 的 FLM 文件）

仓库中的 FLM 文件是从对应 MCU 官方提供，对应 MCU 文件夹中里面会有相应的下载地址及说明。

根据 [Segger 对 JLinkDevices 文件夹](https://wiki.segger.com/J-Link_Device_Support_Kit#JLinkDevices_folder) 的说明：

```bash
jlink-software-and-documentation >= 7.62
```

| OS      | Location
|---------|---------
| Windows |C:\Users\<USER>\AppData\Roaming\SEGGER\JLinkDevices
| Linux   | $HOME/.config/SEGGER/JLinkDevices
| macOS   | $HOME/Library/Application Support/SEGGER/JLinkDevices

```bash
\---JLinkDevices
    +---Vendor1
    |   +---DevFamily1
    |   |       Devices.xml
    |   |
    |   +---DevFamily2
    |   |       Devices.xml
    |   |
    |   \---DevFamily3
    |           Devices.xml
    |
    +---Vendor2
    |   +---DevFamily1
    |   |       Devices.xml
    |   |
    |   +---DevFamily2
    |   |       Devices.xml
    |   |
    |   \---DevFamily3
    |           Devices.xml
    |
    \---Vendor3
        +---DevFamily1
        |       Devices.xml
        |
        +---DevFamily2
        |       Devices.xml
        |
        \---DevFamily3
                Devices.xml
```

## Arch Linux 下使用

```bash
yay -S mcu-jlink-pack
yay -S holtek-jlink-pack
yay -S hkmicrochip-jlink-pack
```
