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

skanda.huayan
2020.12.22


