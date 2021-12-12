# Robosys_device_driver
_________________________
ロボットシステム学2021課題1

:
Raspberry Pi 4 でLEDを制御。


#　動作環境
___________

OS：Ubuntu20.04server


ハードウェア：Raspberry Pi 4


#　インストール・ビルド方法
___________________________

1.git clone https://github.com/Ryoya1012/Robosys_device_driver.git


2.cd robosys_device_driver


3.make


4.sudo insmod myled.ko


5.sudo chmod 666 / dev/myled


#　実行方法
___________

点灯


echo 1 > /dev/myled0


消灯


echo 0 > /dev/myled0



#　ドライバのアンインストール
_____________________________

sudo rmmod myled



#　実行結果
___________

以下のリンクからyoutubeの動画がご覧できます


https://youtu.be/VcskahKzksw


#　参考
_________

以下の動画を参考にしました。


https://youtu.be/xQW8-FNuboo
