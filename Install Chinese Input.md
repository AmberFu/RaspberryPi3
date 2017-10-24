## 安裝中文輸入法 - IBUS 新酷音

* 1. 於對 ibus 印象很好，因此在設定 Raspbian Stretch 環境時，仍選擇新酷音做為中文輸入法。

```
$ sudo apt-get install ibus-gtk ibus-qt4 ibus-chewing 
```

其他常見輸入法： [IBUS](https://github.com/ibus/ibus/wiki/ReadMe)

```
$ sudo apt-get install ibus-zhuyin #注音輸入法
$ sudo apt-get install ibus-table-cangjie-big #倉頡輸入法
$ sudo apt-get install ibus-table-emoji #輸入表情符號
```

* 2. 重啟 ibus : 載入剛安裝的輸入法。

```
$ ibus restart
```

* 3. 啟動 IBus ：

    - 3-1a. Terminal :
      ```
      $ /usr/bin/ibus-daemon --xim &
      $ /usr/bin/ibus-setup
      ```
      （開啟設定界面）
      
    - 3-1b. 視窗界面：
     開始 -> Preferences -> IBus Preferences （開啟設定界面）
    
    - 3-2. IBus Preferences：
        - General : 可設定切換鍵
        - Input Method : Add -> Chinese -> Chewing （新增輸入方式）
        - Close 完成設定
        

完成後，在右上角 EN 部份，點擊可以看到 新酷音 選項。
