Automated Sheet Handling System

This repository contains the Arduino code for an Automated Sheet Handling System that performs a series of tasks using motors, limit switches, an ultrasonic sensor, a servo motor, and other components. The system automates the movement, sealing, and suction processes for handling sheets or similar materials.

Features

Ultrasonic Distance Measurement: Measures the distance to the object using an ultrasonic sensor and triggers actions accordingly.

Motorized Movement: Controls two motors via the BTS7960 motor driver for forward and backward motion.

Servo Control: Operates a servo motor to lock and release the cover.

Sealing Mechanism: Activates a sealer for sealing operations.



Limit Switch Integration: Uses limit switches to determine motor stop points and trigger specific actions.


Components Used

Arduino Uno/Nano (or compatible board)

BTS7960 Motor Driver Module (2 modules for two motors)

28BYJ-48 Stepper Motor (or any compatible motor)

Servo Motor

Ultrasonic Sensor (HC-SR04)

Limit Switches (4 switches)

Sealer (activated using a digital pin)


Resistors and other supporting electronics.


Pin Configuration

Functionality

1. Distance Measurement:

Measures the distance to the object using the ultrasonic sensor.

Triggers different actions based on the measured distance.



2. Motor Control:

Moves the sheet forward and backward using two motors controlled by the BTS7960 motor drivers.

Stops the motors when limit switches are triggered.



3. Servo Motor Operation:

Locks and releases the cover during the process.



4. Sealing:

Moves the sealing mechanism forward and performs the sealing operation.

Moves the mechanism back to its original position after sealing.








How to Use

1. Hardware Setup:

Connect the components as per the pin configuration table.

Ensure the power supply is sufficient for the motors and other peripherals.



2. Code Deployment:

Download and open the code in the Arduino IDE.

Select the correct board and port in the IDE.

Upload the code to the Arduino board.



3. Operation:

Place the sheet/material in the appropriate position.

The system will automatically perform the actions based on the ultrasonic sensor readings and limit switch states.




Dependencies

Servo.h: Library for servo motor control.

BTS7960.h: Library for controlling the BTS7960 motor driver (must be included in your Arduino libraries).


Notes

Ensure all connections are secure before powering the system.

Adjust motor speeds and delays as needed to match your specific setup.


Debugging

Use the Serial Monitor in the Arduino IDE to view debug messages and sensor readings.

Ensure all sensors and motors are properly calibrated.




Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

Author

mdeniston2003@gmail.com
Email Me for any queries.
