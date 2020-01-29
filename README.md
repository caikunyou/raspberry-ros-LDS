# raspberry-ros-LDS

HLS-LFCD2

#必要物：\
       raspberry 3B+ \
       USB to TTL USB (CP2102)\
![image](https://github.com/caikunyou/raspberry-ros-LDS/blob/master/img/20200130021345.jpg)
       Hitachi-LG (HLS-S-LFCD2)\
![image](https://github.com/caikunyou/raspberry-ros-LDS/blob/master/img/20200130021406.jpg)
#接線方法\

Hittachi-LG---------->USB to TTL\
Vcc--------------------->5V\
TX---------------------->RX           \
PWM           \
GND--------------------->GND           \
RX---------------------->TX           \
BOOT0           \
           
モータ側 --------Hittachi-LG           \
Vcc------------->Vcc           \
PWM------------->PWM           \

使ったOS https://downloads.ubiquityrobotics.com/pi.html

#install方法
```$  cd /catkin_ws/src/
$  git clone https://github.com/caikunyou/raspberry-ros-LDS.git
$  cd  ~/catkin_ws
$  catkin_make
$  source ~/catkin_ws/devel/setup.bash
$  cd
テスト
$  roslaunch hls_lfcd_lds_driver hlds_laser.launch
scanテスト
$  roslaunch hls_lfcd_lds_driver view_hlds_laser.launch
```
![image](https://github.com/caikunyou/raspberry-ros-LDS/blob/master/img/20200130023256.jpg)

YouTube　　https://youtu.be/jjwV9W1ukl4  \
参考資料　  https://blog.csdn.net/jacka654321/article/details/83043031  \
