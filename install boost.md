# how to install boost by vs2008

1. download & unzip

    download it from github or boost.org,unzip to anywhere you like.

2. 配置cl环境变量
    
    先在控制台测试 `cl` 命令，没有的话找到cl.exe，把它的目录添加到 `Path` 系统环境变量中。

3. 编译

    使用 `visual studio 命令提示符`，转到boost解压所在的目录（先跳转到该盘，直接盘符如 `d:`） ，然后控制台执行 `bootstrap.bat` ，当前文件夹生成 `b2.exe` 和 `bjam.exe`。

4. 控制台继续执行：

    >b2.exe stage --toolset=msvc-9.0 address-model=64 --stagedir="D:\项目工程文件\boost\bin1.64.0\VC9.0" threading=multi --build-type=complete --build-dir="D:\项目工程文件\boost\build"

    注意修改路径
