# Formate SD card

1. 用 df -h 指令，取得 SD 卡掛載位置：

```
$ df -h
Filesystem     1K-blocks     Used Available Use% Mounted on
:
:
/dev/sda1        58G  3.1G   55G   6% /media/amberfu/B1C4-01F1
/dev/mmcblk0p2   30G  5.6G   23G  20% /media/amberfu/b4ea8e46-fe87-4ddd-9e94-506c37005ac5
/dev/mmcblk0p1   42M   21M   21M  51% /media/amberfu/boot

```
其中， USB 為 /dev/sda1 , SD 卡為 /dev/mmcblk0p1 & p2

2. 卸載 SD 卡：

```
$ sudo umount /dev/mmcblk0

```

3. 格式化 SD 卡：

```
$ sudo mkfs.vfat /dev/mmcblk0 
mkfs.fat 3.0.28 (2015-05-16)
```
將 SD 卡格式化成 FAT32 格式。

4. 退出再插入 SD 卡， 用 df -h 確認格式化成功：

```
$ df -h
Filesystem      Size  Used Avail Use% Mounted on
:
:
/dev/sda1        58G  2.5G   56G   5% /media/amberfu/B1C4-01F1
/dev/mmcblk0     15G  8.0K   15G   1% /media/amberfu/5F89-2A8A

```

# Write OS into SD Card

1. 下載 Raspberry Pi OS : 

  * 官網： https://www.raspberrypi.org/downloads/


2. 下載 Etcher Img 燒錄軟體： (Mac,Linux,Windows)

  * 官網： https://etcher.io/

3. 解壓縮 OS ：

xxx.img.gz 用 gunzip 解壓縮

4. 使用 Etcher 燒錄：

參考 Etcher_write_OS.png 

ps. 或參考 https://elinux.org/RPi_Easy_SD_Card_Setup 用 CML 燒錄


