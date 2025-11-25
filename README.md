This project implements a closed-loop control system to ensure a 4-wheel robotic vehicle drives in a straight line.
The platform is based on an Arduino Nano microcontroller, paired with a custom motor driver board, four DC motors equipped with rotary encoders, and an MPU-6050 IMU.

The control algorithm continuously measures the vehicle’s yaw angle using the MPU-6050.
Any yaw deviation is translated into speed offsets for the left and right wheel groups.
This enables real-time heading correction and maintains straight-line motion on uneven surfaces.

Reference
This project was inspired by the following video:
YouTube: https://www.youtube.com/watch?v=LfydfvHyikM&list=LL

Yaw Measurement Source
The yaw value is obtained using the MPU-6050 DMP (Digital Motion Processor).
The implementation is based on the following example code from Electronic Cats:

GitHub:
https://github.com/ElectronicCats/mpu6050/blob/master/examples/MPU6050_DMP6/MPU6050_DMP6.ino
The implementation of closed-loop motion control and yaw-based correction follows concepts demonstrated in the video, then adapted and optimized for my own hardware platform.
