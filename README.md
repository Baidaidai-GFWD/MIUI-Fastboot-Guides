# MIUI刷机指南(新手向)
### 什么是刷机，卡刷和线刷是什么
请注意，这里指的确实是`字面意思`</br>
- `卡刷`顾名思义就是用卡(<del>SD卡</del>)来进行刷机</br>
由于以前的安卓机基本都是用MicroSD卡来进行刷机，顾称卡刷</br>
由于技术水平的提升，现在Android设备都内置了虚拟SD卡可以进行徒手刷机</br>
故`卡刷`为`脱离电脑，仅凭Android设备即可完成刷机的一个刷机方式`
- `线刷`顾名思义就是`用数据线`连接电脑进行刷机操作
- <del>(这里以MIUI刷机包举例) </del>其中卡刷的刷机包后缀一般为`.zip`而线刷包的后缀一般为`.tgz`
### 我要进行刷机前，需要做什么
如果你的手机没有任何问题，不建议进行刷机！！</br>
如果你的手机没有任何问题，不建议进行刷机！！</br>
如果你的手机没有任何问题，不建议进行刷机！！</br>
1. 你需要一步bootloader解锁过的设备
2. 需要准备一个官方的刷机包(线刷最好，尽量用官方的</br>
以免刷机包格式错误以免被人恶意植入`后台木马`)
3. 你需要一根`数据线`
### 那选择了线刷包后，我应该怎么操作？(以MIUI举例)
1. 解压`.tgz`格式的线刷包(winrar或者360压缩都可以) 
- 在这一步，你可以选择用`MiFlash官方刷机工具`或者徒手进行`手动刷机`(接下来我以手动刷机举例)
2. 打开线刷包，找到`FlashAll.bat`或`FlashAll.sh`(sh为Linux格式的刷机脚本，bat为Windows格式的刷机脚本)
3. 打开系统`终端`(Windows为Cmd)拖入刷机脚本并`执行`
4. 等待刷机脚本执行完毕重启
### 为什么不推荐卡刷包
1. `从MIUI10`(可能是)开始，解除Bl锁的设备`均无法`在`Recovery`界面进行选择刷机包进进行刷机操作
2. 由于机型数量庞大，`第三方Recovery`无法及时适配，刷机难度`陡然增加`
3. 通常情况下，如果您的设备能`出现问题`，Recovery将`无法进入`
4. Fastboot较Recovery刷机会`更纯净`
### 通常情况下的崩溃及解决办法
- konabess调度过大黑屏：刷入vendor_boot.img
- magisk模块出错：刷入boot.img
- kernelsu内核错误：刷入boot.img