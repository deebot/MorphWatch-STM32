# MorphWatch-STM32
Morph watch is a wearable made for makers and hackers who want to do more with  their devices and want to have control over their data. As a normal functional device it shows time, date and no of steps,weather data . But it is more than that it can be used to run machine learning algorithums on 6 Axis IMU MPU6050 data to detect gestures. The small form factor and integrated battery also allows the user to attach the watch to a target lets say attach it to your bicycle to gather the vibration data, or attach it to a machine to gather the vibration data to  train a model for predicting breakdown and service durations. The device also  provides I2C interface to attach more sensorS as modules. The device also provides interface  to connect with  STLINK-V2 and supports full debugging features using breakpoints and print statements. The watch is intended to have 2 Modes:

- Ultra Low Power Mode : In this mode the L476RG controller  wakes up ever 1 minute to update the minutes and then sleeps. The 2 buttons are configures as external intrupts and can be pressed to wake up the controller and do other tasks like going though the Menu  and getting the status of external senors or accelerometer data. This mode should give very long battery life

- Normal Mode: In this mode the microcontroller is active all the time and can count steps and perform machine learning algorithums.


