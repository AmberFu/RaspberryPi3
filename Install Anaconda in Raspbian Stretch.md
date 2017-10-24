## 在 Raspbian Stretch 安裝 Anaconda

1. 到 [Anaconda](https://www.anaconda.com/download/#linux) 下載 Installer

本次安裝版本為：
Anaconda 5.0.0 For Linux Installer
Python 3.6 version * 
32 bit 

```
$ sudo wget https://repo.continuum.io/archive/Anaconda3-5.0.0.1-Linux-x86.sh
```
檔案有 430M ，下載需要花一些時間。

2. [Installing on Linux](https://docs.anaconda.com/anaconda/install/linux)

Install Anaconda for Python 3.6 :
```
$ bash ~/PATH_YOU_SAVE/Anaconda3-5.0.0.1-Linux-x86.sh
```
3. 同意 license ，並依提示同意安裝…

```
Anaconda3 will now be installed into this location:
/home/pi/anaconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below
  
[/home/pi/anaconda3] >>> 
PREFIX=/home/pi/anaconda3
installing: python-3.6.2-hbf0f4e3_15 ...
Anaconda3-5.0.0.1-Linux-x86.sh: line 354: /home/pi/anaconda3/pkgs/python-3.6.2-hbf0f4e3_15/bin/python: cannot execute binary file: Exec format error

```
--> 無法成功安裝！！！ QQ


~~4. 同意將路徑加入 PATH，安裝完成會會看到 “Thank you for installing Anaconda3!”~~


 
