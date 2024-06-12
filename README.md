---

<h1 align="center">Line Follower Robot</h1>

> [!NOTE]
> ### This is the code being used on `TRAILBLAZER` v3.1.0 `~By Team Cyclops`
> 
> All the rights are reserved strictly by Team Cyclops for the members of the team 
> for enquiries and implementation only. Any further implementations to LFR and variation to code will be available on this repository in dedicated branches.

---

# Line Follower Robot using Arduino Uno

This project demonstrates a line follower robot powered by an Arduino Uno. The robot uses infrared (IR) sensors to detect the line and adjust its path accordingly by controlling the motors.

## Table of Contents
- [Introduction](#introduction)
- [Components](#components)
- [Circuit Diagram](#circuit-diagram)
- [Code Explanation](#code-explanation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contacts](#contacts)

## Introduction
The line follower robot is designed to follow a black line on a white surface. It uses five IR sensors to detect the line's position and adjusts its movements by controlling the left and right motors accordingly.

## Components
- Arduino Uno R3
- 2 DC Motors with motor driver
- 5 IR Sensors (individual or array chanel works)
- Motor driver (L298N or similar)
- Chassis, wheels, and other mechanical components
- Jumper wires (breadboard is optional)

## Circuit Diagram
[Insert an image or a link to the circuit diagram here]

## Code Explanation
The code is designed to:
- Read the values from five IR sensors.
- Determine the position of the line based on the sensor values.
- Adjust the motor speeds to follow the line correctly.

### Motor Control
- `motorRPin1`, `motorRPin2`, and `motorREnable` control the right motor.
- `motorLPin1`, `motorLPin2`, and `motorLEnable` control the left motor.

### IR Sensors
- The IR sensors are connected to analog pins A0 to A4.

### Functions
- `scanD()`: Reads the IR sensor values.
- `check()`: Determines the robot's movement based on the sensor values.
- `rightS()`, `leftS()`, `go()`, `stopme()`: Control the motors to turn right, turn left, move forward, and stop respectively.

## Inbuilt Functions
-  `analogWrite()`: Allows you to write a an analog value (a pulse-width-modulation wave) to a specific pin.
     ```INO
      Syntax:
      analogWrite(pin, value)
      Parameters:
      Pin - Pin to write to allowed to be an int only
      value -  The duty cycle, ranging from 0 to 255 
     ```
-  `digitalWrite()`:
-  `bitWrite()`:

## Usage
1. **Assemble the Hardware**:
   - Connect the IR sensors to the analog pins A0 to A4 on the Arduino.
   - Connect the motor driver to the Arduino and the motors.
   - Power the Arduino and motor driver.

2. **Upload the Code**:
   - Upload the provided code to the Arduino Uno using the Arduino IDE.

3. **Run the Robot**:
   - Place the robot on a track with a black line on a white surface.
   - The robot will follow the line autonomously.

## Contributing
We welcome contributions to improve the project. Here’s how you can contribute:
- Fork the repository.
- Create a new branch (`git checkout -b feature-branch`).
- Commit your changes (`git commit -am 'Add new feature'`).
- Push to the branch (`git push origin feature-branch`).
- Create a new Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contacts
   Nathan Cordeiro 
   ```sh
   https://github.com/NathanCordeiro
   ```
    
   Sanika Naik
   ```sh
   https://github.com/SanikaKNaik
   ```

   Vaidehi Kolhatkar
   ```sh
   https://github.com/VaidehiKolhatkar
   ```



