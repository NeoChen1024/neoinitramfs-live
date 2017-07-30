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

* 建構平台的Glibc必須和config裡的一樣。
* 不支援WIFI上網，沒有瀏覽器。
* 若要在Initramfs裡加入自己的檔案，加到overlay目錄裡。
* 要使用不一樣的套件版本，編輯config。

套件：

+ Linux Kernel
+ Glibc
+ Busybox
+ Sash (Standalone Shell)
+ TCC (Tiny C Compiler)

可用核心參數：

+ noinit	不預設執行Init
+ bootroot	啟動進去root=指定的裝置 （可以用LABEL= 和UUID= ）
