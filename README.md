## The gyro
----------------------------------------
> in this project we are going to learn how to ***use gyro with Arduino ***
> for this project you need to have the lib of `mpu6050 made from electronic cats and the wire.h` lib
>this project has 2 step: first colibration , second the main code
-------------------------------------
## STEPS
1.  if you have download that lib you can find the examples of it  in `file\example\mpu6050`
2. open  `IMU_Zero` in `file\example\mpu6050`
3. now its conection time, the conection is like this:
![This is an image](https://www.electronicwings.com/public/images/user_images/images/Arduino/MPU6050/Arduino%20Gyro.png)
4. now run `IMU_Zero` program (this program will take 5 or 6 minutes, while its runnig please dont touch your gyro)
5. at the end it will  give you some number, past them in a notepad
6. open the `MPU6050_DMP6` and go to 205 line
7. enter that numbers there
##And done!
---------------------------------
> if you can't find `MPU6050_DMP6` and `IMU_Zero` they are in code folder of this repository
> if  you need more imformation you can visit [howtomechatronics](https://howtomechatronics.com/how-it-works/electrical-engineering/mems-accelerometer-gyrocope-magnetometer-arduino/).