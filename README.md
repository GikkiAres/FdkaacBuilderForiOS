# 脚本名称

FdkaacBuilderForiOS

# 使用方法
## 下载源码



## 配置参数

### 配置源码路径

假设libPath为您下载库后放在电脑的路径.

需要在脚本中,设置libPath为该路径.

### 配置要编译的架构

在archs中,设定要编译的架构,默认为"i386 x86_64 armv7 arm64"

## 运行脚本

执行命令,编译Lame库
`sh FdkaacBuilderForiOS.sh`

## 编译结果

该脚本会分别在
libPath/../Build/Thin/x86_64
libPath/../Build/Thin/i386
libPath/../Build/Thin/armv7s
libPath/../Build/Thin/arm64
四个目录中,编译对应平台下的库文件
然后将四个平台下的库合并到
libPath/../Build/Fat中

实际使用时,我们只要把fat中的.a库文件和头文件一起拷贝到项目中去就可以了.

# 版本记录

## 0.0.5(10)

UpdateTime

2020-11-18

Content:

针对Fdkaac 2.0.1进行测试,可用.

