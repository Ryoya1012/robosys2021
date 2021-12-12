# Robosys_device_driver
ロボットシステム学2021課題1

Raspberry Pi 4 でLEDを制御した。


動作環境


OS：Ubuntu20.04server


ハードウェア：Raspberry Pi 4

インストール・ビルド方法


git clone https://github.com/Ryoya1012/Robosys_device_driver.git


cd robosys_device_driver


make


sudo insmod myled.ko


sudo chmod 666 / dev/myled

実行方法


点灯


echo 1 > /dev/myled0


消灯


echo 0 > /dev/myled0





ドライバのアンインストール


sudo rmmod myled





実行結果


以下のリンクからyoutubeの動画がご覧できます





参考
 



以下の動画を参考にしました。


https://cit.manaba.jp/ct/link_iframe_balloon?url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DxQW8-FNuboo
