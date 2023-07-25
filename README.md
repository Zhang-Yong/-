# 轮腿机器人上位机控制板
轮腿机器人上位机控制板，ESP32 lion32 lite controlled board, 模块化设计，包括5V,3V3电源，MPU6050，I2C 1.3inch 显示模块
Version 1.0, tested work. May Optimize Ams1117, MPU6050 location, put OLED in the front


Version 2.0. 更新。 7/25
修改MPU6050 GPIO 管脚，修改SDA 连接为ESP32 lion32 lite 的GPIO. 
下位机串口通讯调试通过。 7/25
下位机为电机FOC控制板，用ESP32，支持WIFI, BLE通讯, 采用双电压供电方式，优点， 待机功耗小，缺点，通讯时需要12v 电源给USB电路上电。如果用CAN就不需要，但更新FOC fireware 需要。
修改下位机FOC firmware，disable T command set voltage echo output. 上位机获取motor速度和角度时不会引入echo 的 set control voltage 电压值。
支持上下位机CAN 接口通讯， 待调试。完成后可以去掉串口线。

