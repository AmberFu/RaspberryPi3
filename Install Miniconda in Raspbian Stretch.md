## 在 Raspbian Stretch 安裝 Miniconda

由於安裝 Anaconda 失敗（下方有失敗紀錄...），改成安裝 Miniconda，
但要注意必須安裝 ARMv71 版，目前看來此版本僅更新到 2015/08/24 。

Filename | Size | Last | Modified	MD5 
-------- | ---- | ---- | ------------
Miniconda3-latest-Linux-armv7l.sh	| 29.9M |	2015-08-24 12:34:00	| a01cbe45755d576c2bb9833859cf9fd7


1. 到 [Miniconda installer archive](https://repo.continuum.io/miniconda/index.html) 下載 Installer

本次安裝版本為：
Miniconda3 For Linux-armv71 Installer
Python 3 version

```
$ sudo wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-armv7l.sh
```
檔案僅有 49M 。

2. [Use bash to install](https://conda.io/docs/user-guide/install/index.html)

Install Miniconda for Python 3.6 :

```
$ bash ~/PATH_YOU_SAVE/Anaconda3-5.0.0.1-Linux-x86.sh
```
閱讀並同意 license ，並依提示同意安裝…

```
Do you approve the license terms? [yes|no]
[no] >>> yes

Miniconda3 will now be installed into this location:
/home/pi/miniconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/pi/miniconda3] >>> 
PREFIX=/home/pi/miniconda3
installing: python-3.4.3-1 ...
installing: python-3.4.3-1 ...
installing: conda-env-2.4.2-py34_0 ...
installing: openssl-1.0.1k-1 ...
installing: pycosat-0.6.1-py34_0 ...
installing: pyyaml-3.11-py34_1 ...
installing: requests-2.7.0-py34_0 ...
installing: sqlite-3.8.4.1-1 ...
installing: xz-5.0.5-0 ...
installing: yaml-0.1.6-0 ...
installing: zlib-1.2.8-0 ...
installing: conda-3.16.0-py34_0 ...
installing: pycrypto-2.6.1-py34_0 ...
Python 3.4.3 :: Continuum Analytics, Inc.
creating default environment...
installation finished.
Do you wish the installer to prepend the Miniconda3 install location
to PATH in your /home/pi/.bashrc ? [yes|no]
[no] >>> yes

Prepending PATH=/home/pi/miniconda3/bin to PATH in /home/pi/.bashrc
A backup will be made to: /home/pi/.bashrc-miniconda3.bak


For this change to become active, you have to open a new terminal.

Thank you for installing Miniconda3!

```
完成！


## 在 Raspbian Stretch 安裝 Anaconda [失敗，不支援 ARMv71 晶片]

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
閱讀並同意 license ，並依提示同意安裝…

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


~~3. 同意將路徑加入 PATH，安裝完成會會看到 “Thank you for installing Anaconda3!”~~


 
