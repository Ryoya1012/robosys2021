# Robosys_device_driver

ロボットシステム学2021課題1
______

# はじめに


 ご覧いただきありがとうございます。このプログラムは、講義内で作成したデバイスドライバのコードです。
以下に、クローン・動作方法を記しましたので、ライセンスに沿ってご利用ください。
また、このコード作成はDaiki414のRaspberry Pi 4をお借りして作成したものになります。
このコードは、Raspberry Pi 4 でLEDを制御するものです。


# 動作環境


|OS| Ubuntu20.04server |
---|---
|Hardware|Raspberry Pi 4|


# 使用するもの


・ブレッドボード


・ジャンパーワイヤー
　　（オスーメス　２本）


・LED　１個


・抵抗200Ω １個


# 回路


GPIO25(22番ピン)にLEDのアノード側を繋げる。


LEDのカソード側をGND(39番ピン)に繋げる。その際に、抵抗を間につなげる。


# インストール・ビルド方法


1.git clone https://github.com/Ryoya1012/Robosys_device_driver.git
 

2.cd robosys_device_driver


3.make
 ->コンパイル

4.sudo insmod myled.ko
 ->ドライバをインストールする

5.sudo chmod 666 / dev/myled
->権限付与するため

# 実行方法


点灯


echo 1 > /dev/myled0


->myled.c 内で変更可能

消灯


echo 0 > /dev/myled0


->myled.cで変更可能

# ドライバのアンインストール


sudo rmmod myled



# 実行結果

以下のリンクからyoutubeの動画がご覧できます


https://youtu.be/VcskahKzksw


# 参考


以下の動画を参考にしました。


https://youtu.be/xQW8-FNuboo
