# 概要
ロボットシステム学で作ったデバイスドライバです。  
講義のプログラムに少し付け加えたものです。一緒にやった人はいないです。  
LEDの点滅の間隔がだんだん遅くなっていくプログラムで、11回点滅を繰り返した後点灯したままになります。    　

# 動作環境
raspberry Pi 4 Model B 　　  
ubuntu 18.04 　　  


# デモ動画のリンク
https://youtu.be/W8AW6gRROx4

# 実行方法
$make  　
$sudo insmod myled.ko  
$sudo chmod 666 /dev/myled0 　　  

# 動作
$echo 0 > /dev/myled0 　
LEDの消灯 　　 

$echo 1 > /dev/myled0 　  
LEDが点滅後、点灯 　　  
 
# ライセンス
GPL v3.0
