# NeoInitramfs

就是一個奇怪的Live Initramfs建構腳本
從零開始建構一套不正常的Live系統

大部分Written from Scratch
udhcpc的helper和rc.dhcp是從Minimal Linux Live那裡借來用的

純粹好玩

設定檔：config  
建議建構平台：Arch Linux

靈感來源：[Minimal Linux Live](https://github.com/ivandavidov/minimal)

注意事項：

* 暫時沒有加入自動dhcp設定網路的計畫。
* 若要在Initramfs裡加入自己的檔案，加到overlay目錄裡。
* 要使用不一樣的套件版本，編輯config。

套件：

+ Linux Kernel
+ Glibc
+ Busybox
+ Sash (Standalone Shell)

