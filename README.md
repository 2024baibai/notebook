# centos安装PyV8
0. 安装gcc
```
yum install gcc gcc-c++
```
1. 安装boost：
```
wget https://dl.bintray.com/boostorg/release/1.65.1/source/boost_1_65_1.tar.gz
tar -zxvf boost_1_65_1.tar.gz  #解压比较长时间
cd boot_1_65_1
./bootstrap.sh
./b2
```
2. 下载pyv8编译包，解压对应版本的压缩包，并将PyV8.py和_PyV8.so移动到site-packages目录下
```
git clone https://github.com/emmetio/pyv8-binaries
cd pyv8-binaries
unzip pyv8-linux64.zip 
mv PyV8.py _PyV8.so /usr/lib/python2.7/site-packages
```

测试！