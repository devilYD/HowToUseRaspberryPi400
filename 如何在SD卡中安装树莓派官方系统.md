# 如何在SD卡中安装树莓派官方系统

树莓派400的官方套件中包含有一张已经装好Raspberry Pi OS(树莓派操作系统)的 SD 卡，一般是不需要对它做过多的修改的，但如果您需要更换新的更大容量的 SD 卡(不推荐这么做，因为SD卡非常容易损坏)，或者您的原装 SD 卡(请允许我这么称呼它)已经发生了损坏，则可按照本教程在新的 SD 卡中安装Raspberry Pi OS。

*本教程参考[Raspberry Pi官方教程编写](https://www.raspberrypi.com/software/)。*

## 安装前的准备

在进行系统的安装以前，您首先需要下载一个专用软件，即树莓派官方提供的工具软件Raspberry Pi Imager，官方下载地址如下：

* [适用于windows系统](https://downloads.raspberrypi.org/imager/imager_latest.exe)
* [适用于macOS系统](https://downloads.raspberrypi.org/imager/imager_latest.dmg)
* [适用于x86架构的Ubuntu系统](https://downloads.raspberrypi.org/imager/imager_latest_amd64.deb)

另外如果是适用于Raspberry Pi OS则可以直接在终端下输入如下命令：

```shell
sudo apt install rpi-imager
```

这个工具软件的主要功能就是将Raspberry Pi OS的映像写入指定的SD卡中。

除了这个软件，还需要下载Raspberry Pi OS的映像文件到您的电脑上，才能开始安装。

可以直接从[Raspberry Pi OS官方下载地址](https://www.raspberrypi.com/software/operating-systems/)选择合适的系统下载，为方便在国内使用，推荐下载Raspberry Pi OS (64-bit)的Raspberry Pi OS with desktop版本，这是由于国内有些大型互联网企业的产品对linux的适配做的稀烂导致32位系统无法使用他们开发的软件。

## 将Raspberry Pi OS映像写入 SD 卡

安装Raspberry Pi Imager到您的电脑(这里没有什么特殊选项，一路Next就好了)。

将您将与 Raspberry Pi 一起使用的 SD 卡放入读卡器并接入电脑。

打开Raspberry Pi Imager，点击最左侧按钮，浏览文件目录并选择刚刚下好的系统映像，然后点击中间的按钮选择您的 SD 卡，注意一定要确认容量以确保您选择的是您的 SD 卡而不是您其他的外部储存设备，最后点击最右边的按钮进行烧录。

等待一段时间。

将烧录完成的 SD 卡插回您的树莓派400的卡槽中，并启动您的树莓派。

等待初始化，并根据自己的需求设置初始值。

完成。