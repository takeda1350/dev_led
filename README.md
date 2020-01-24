# dev_led
## 概要  
モールス信号で自分の名字をLEDを点灯させる
## インストール方法  
```
$ https://github.com/yoshiken5586/dev_led.git
```
## 実行方法
```
$ cd dev_led
$ make  
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0  
```
デバイスファイルに`1`を書き込むとモールス信号が点滅する
```
$ echo 1 > /dev/myled0
```
## 後処理  
以下のコマンドでデバイスファイルを削除する　　
```
$ sudo rmmod myled
```

## ライセンス  
This repository is licensed under the GPLv3 license, see COPYING.
