# Panopticron
#### A robot based on stabilization system self-balancing motorcycle using Cortex-M0. 

## Description
Using the GreenPill - STM32F030F4P6 which is a Microprocessor incorporates the high-performance ARM Cortex - M0 32-bit RISC core for create a robot with stabilization control system of self-balancing. This self-balance robot is made by subassemblies: 

* The first one is mpu 6050 which is a module of Gyro + Accelerometer which can sens any tiny movement convert it in to signal and transmit it into the controler after that the controler will process the signal and respond to it this respond signal will go to the motor driver and convert to the level of voltage, the voltage leavel determines how the motor moves at the same time  will give feedback to the controller so, its the Gyro + Accelerometer sensor will determine the balance of the robot. This is the mechanical principle in order to achieve auto-balance.

* The second are two algorithms that should to apply to the controler,   the first on is Kalman Filtering it can filter out the interference signal in the waveform where the movement of the robot will smooth and consistence and the second algorithm, is the PID algorithm, the PID stands for  proportional intergral derivative mode, this algorithm provide the car the ability to predict actions and the ability to adjust their posture. 

It’s important to mention that the angle data needs to be filter because the system will always shock in the process of motion, what makes an interference with the MPU. The Kalman filtering algorithm used to be applied to process data algorithm in the field of automatic control, it’s your biggest area. It’s important to mention that the system’s external disturbances and observation errors, assuming the system could predicted the value and the measured value, which represent the real value combined with the noise, respectively. In that way, the most close value next to the real signal can be obtained.


## Components
* Microprocessor: GreenPill - Cortex M0
* Module: accelerometer & gyroscope - MPU_6050
* 2 Motors
* Driver Motor
* Battery

## Group
* Kayann Costa Soares
* Luan Alves Cruz
* Glauton Cardoso Santos

