# 使用 adb 授权软件 Sam Helper<br>
<br>

## ❇️准备工具

1. [ADB 工具包](https://github.com/MagicCD/Authorization-ADB/blob/main/platform-tools/platform-tools.zip)
2. 软件 Sam Helper

***
<br>

## 🌟授权步骤

1. 使用电脑先下载好 [ADB 工具包](https://github.com/MagicCD/Authorization-ADB/blob/main/platform-tools/platform-tools.zip)，并解压到你能找到的文件目录中
2. 点开 设置——关于手机——软件信息——多次点击编译版号，直至出现开发者选项已启用字样
3. 用数据线把手机和电脑链接
4. 点开开发者选项，找到 USB 调试，点击打开
   + 如果出现是否允许USB调试，点击确定，并勾选 `一律允许使用这台计算机进行调试`

5. 找到解压后的 ADB 工具包，确认是否有 `adb.exe`，如果没有请重新解压或下载

6. 定位于文件目录下，如下图所示操作，进入 cmd命令运行窗口

<img src="使用 adb 授权 Sam Helper.assets/image-20220209021706475.png" alt="image-20220209021706475" style="width:70%;" /> 

<br>

输入 `adb devices` 并回车。此时手机会出现弹窗，点击确定并勾选 `一律允许使用这台计算机进行调试`

+ 此时电脑会出现设备链接的列表，代表进入调试状态

<img src="使用 adb 授权 Sam Helper.assets/Screenshot_20220209020815.jpg" alt="Screenshot_20220209020815" style="width: 40%;" /> <img src="使用 adb 授权 Sam Helper.assets/image-20220209022103097.png" alt="image-20220209022103097" style="width: 57%;" /><br>



7. 打开软件 Sam Helper 获得授权代码

~~~bash
adb shell pm grant com.litebyte.samhelper android.permission.WRITE_SECURE_SETTINGS
~~~

<img src="使用 adb 授权 Sam Helper.assets/image-20220209015112298.png" alt="image-20220209015112298" style="width: 33%;" /> <br>

8. 将此代码复制到 cmd命令窗口，按下回车即可完成授权

<img src="使用 adb 授权 Sam Helper.assets/image-20220209022600103.png" alt="image-20220209022600103" style="width:80%;" />
