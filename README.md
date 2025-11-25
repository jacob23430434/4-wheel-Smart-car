This project implements a closed-loop control system to ensure a 4-wheel robotic vehicle drives in a straight line.
The platform is based on an Arduino Nano microcontroller, paired with a custom motor driver board, four DC motors equipped with rotary encoders, and an MPU-6050 IMU.

The control algorithm continuously measures the vehicle’s yaw angle using the MPU-6050.
Any yaw deviation is translated into speed offsets for the left and right wheel groups.
This enables real-time heading correction and maintains straight-line motion on uneven surfaces.
