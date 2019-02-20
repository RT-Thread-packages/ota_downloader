# OTA Downloader

## 1、介绍

OTA Downloader 是与 OTA 服务器对应的客户端程序，用于将 OTA 固件从 OTA 服务器下载到设备。常用的且通用的 OTA Downloader 有 Y-modem（串口升级） 和 HTTP OTA（网络升级），开发者使用自己的电脑既可搭建用于 OTA 升级的服务端。私有云或者公有云平台提供的 OTA 服务器，通常需要开发对应的客户端程序，运行在设备端，用于下载 OTA 固件。

### 1.1 目录结构

| 名称 | 说明 |
| ---- | ---- |
| docs  | 文档目录 |
| examples | 例子目录，并有相应的一些说明 |
| inc  | 头文件目录 |
| src  | 源代码目录 |

### 1.2 许可证

OTA Downloader package 遵循 LGPLv2.1 许可，详见 `LICENSE` 文件。

### 1.3 依赖

- RT-Thread 3.0+
- fal 软件包支持
- Y-modem 下载方式依赖于 Y-modem 组件
- http 下载方式依赖于 webclient 软件包

## 2、如何打开 OTA Downloader

使用 ota_downloader package 需要在 RT-Thread 的包管理器中选择它，具体路径如下：

```
RT-Thread online packages
    miscellaneous packages --->
        [*] ota_downloader
```

然后让 RT-Thread 的包管理器自动更新，或者使用 `pkgs --update` 命令更新包到 BSP 中。

## 3、使用 OTA Downloader

在打开 ota_downloader package 后，当进行 bsp 编译时，它会被加入到 bsp 工程中进行编译。

* 完整的 API 手册可以访问这个[链接](docs/api.md)
* 更多文档位于 [`/docs`](/docs) 下，使用前 **务必查看**

## 4、注意事项

> 说明：列出在使用这个 package 过程中需要注意的事项；列出常见的问题，以及解决办法。

## 5、联系方式 & 感谢

* 维护：name
* 主页：https://github.com/RT-Thread-packages/hello
