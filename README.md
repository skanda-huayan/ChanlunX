### 编译项目

在项目根目录下执行以下命令

```
mkdir build
cd build
cmake ..
cmake --build . --config Release
cmake --build . --config Debug
```

### 使用说明
#编译#
前提：安装Visual Studio 2015和最新版CMake。
按上面的步骤编译项目，即可生成ChanlunX.dll。

#使用#
ChanlunX是通达信的缠论插件。需要把三个文件拷贝到通达信的安装目录
的T0002/dlls之下:
ChanlunX.dll
ChanlunX.ini
ChanlunX.txt

其中ChanlunX.dll，绑定在1号DLL
然后添加公式：拷贝ChanlunX.txt，创建新公式，即可。

```
#通達信輸出函數說明#
1 K線方向
2 是否有包含關係的K線
3 包含處理後的K線高點
4 包含處理後的K線低點
5 處理包含信號，方便通達信畫線
6 輸出筆頂底端點
7 線段頂底信號
8 中樞高點數據
9 中樞低點數據
10 中樞起點、終點信號
11 中樞方向數據
```

skanda.huayan
2021.01.21

```
#ChanlunX-DZH輸出函數說明#
大智慧版ChanlunX，一共11個輸出函數，如下：
1 K線包含處理 / KXBH
2 包含處理後的K線高點 / KXBHG
3 包含處理後的K線低點 / KXBHD
4 K線方向 / KXFX
5 處理包含信號，方便畫線 / KXBH2VAR
6 筆頂底 / BI
7 線段頂底 / DUANVAR
8 中樞高點 / ZSZGVAR
9 中樞低點 / ZSZDVAR
10 中樞起點、終點 / ZSSEVAR
11 中樞方向 / ZSFXVAR
```

說明：
1 函數名不帶VAR的，可以直接調用，如：
```
bi:=“suChan@BI”;
```
2 函數名帶VAR的，需要傳入一個參數，例：
```
duan:=“suChan@DUANVAR”(bi);
```

具體使用可以看公式～

纏海一粟
2021.02.28
