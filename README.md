## Design Specifications
![img](http://i.imgur.com/OjhjUpt.png)
####Problem Statement 33: Flying Robot
- The Flying Robot is a hovering robot that possesses the capability to remain flying
directly over an area of interest until a designated mission is complete.
- The airframe is made up of 4 rods that span out from the centre and form an X shaped pattern. Attached to each rod is a DC motor and gear assembly for a propeller.
- The pitch of adjacent propellers is reversed to compensate for counter rotation, making two propeller rotate clockwise and the other two counter clockwise.
- For sensors piezo gyros are placed on the three axis of rotation provide the yaw, pitch and roll angles of the hovering robot for control.
- Gyro sensors outputs are used to adjust the speed of 4 motors to control the flying robot.
- In addition to the gyro sensors, four IR sensors are placed on the robot to detect
obstructions if the robot approaches walls or obstacles.

### Clarifications to the Problem Statement
- The robot is assumed to be already flying and we just have to maintain its stability.
- If an obstacle is detected by any of the 4 IR Sensors, a corresponding LED is switched on, indicating the detection of the obstacle.


# Assumptions made when implementing the design
- The weight of the robot is assumed to be around ~900g (similar to the weight of many do-it-yourself quadcopters available online. So, keeping the ratio of the total thrust required by the motors at full power to the weight of the robot as 2:1, we get the total thrust as 1800g or 450g per motor. That is approximately the same as that of the motor that we chose.
- The flying robot has three degrees of freedom: Yaw, Pitch and Roll, all of which are measured by a piezo gyroscope. Due to the limitation of the ADC, only one gyro input can be converted to digital code and read by the microprocessor at once. But this is overcome due to the speed of the microprocessor, which can process the input at a faster rate than the sampling rate of the piezo gyro chip, and thus can process the inputs of the gyroscopes sequentially.
- We are designing the IR Sensor with the help of an IR transmitting diode, receiver and comparator. On detecting an obstacle, a LED is lighted to denote which IR sensor
detected the obstacle.

# Team
- Abhinav Singh
- Pulkit Agarwal
- Rohan Goel
- Shikhar Saluja

# License
MIT