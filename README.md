# CS350 – Thermostat Project

## Project Overview

This project involved developing a thermostat prototype using Python and a Raspberry Pi. The system monitors the current temperature and compares it to a user-defined setpoint to determine how the thermostat should respond. I worked on implementing temperature monitoring, button controls, a state machine, LED indicators, an LCD display, and serial communication. Through this project, I gained hands-on experience with embedded systems and learned how software interacts with hardware to create a functional system.

## Technologies Used

- **Python** – Used to implement the thermostat logic, process user input, and manage the system's behavior.
- **Raspberry Pi** – Used as the hardware platform to run the program and interface with connected components.
- **GPIO Zero** – Used to handle button inputs and control the red and blue LED indicators.
- **Adafruit AHTx0** – Used to interface with the temperature and humidity sensor.
- **I2C** – Used to communicate with the temperature sensor.
- **Character LCD Library** – Used to control the 16x2 LCD display.
- **PySerial** – Used to configure serial communication through the Raspberry Pi's serial port.
- **Python State Machine Library** – Used to manage the thermostat's heating, cooling, and off states.

## Project Features

### Temperature Monitoring

I implemented functionality to read the current temperature from the connected sensor and convert the reading from Celsius to Fahrenheit. The system compares the measured temperature with the setpoint to determine how the thermostat should respond.

### Setpoint Adjustment

I configured buttons that allow users to increase or decrease the thermostat's setpoint in one-degree increments. The default setpoint is 72 degrees Fahrenheit. This functionality helped me understand how hardware inputs can be used to modify program variables and influence system behavior.

### Heating, Cooling, and Off Modes

I implemented a state machine to manage the thermostat's three operating modes: heating, cooling, and off. A button allows users to cycle between these states. The state machine organizes the program's behavior and determines which LED indicators should be active based on the selected mode and current temperature.

### LED Indicators

I used red and blue LEDs to represent the thermostat's heating and cooling states. The LEDs provide visual feedback based on the relationship between the current temperature and the setpoint. The red LED represents heating, while the blue LED represents cooling. The LEDs pulse or remain illuminated depending on the operating mode and temperature comparison.

### LCD Display

I integrated a 16x2 LCD display to provide information about the thermostat's operation. The display shows the current date and time on one line and alternates between the measured temperature and the thermostat's operating state and setpoint on the other line. This helped me gain experience working with display hardware and presenting sensor data in a readable format.

### Serial Communication

I configured serial communication through the Raspberry Pi's serial port to support sending thermostat status information to an external temperature server. The intended status information includes the operating mode, current temperature, and setpoint. This feature introduced me to communication between an embedded system and an external application.

## Skills Demonstrated

- Python programming and code organization
- Embedded systems development
- Hardware and software integration
- Temperature sensing and unit conversion
- State machine implementation
- GPIO input and output handling
- LED control and pulse-width modulation
- LCD display integration
- I2C and serial communication
- Debugging and troubleshooting
- Problem-solving and iterative development
- Writing readable and maintainable code

## Reflection

Throughout this project, I developed a stronger understanding of how hardware and software interact within an embedded system. I successfully worked on setting up the hardware and integrating the software to implement the thermostat's functionality. I also gained experience working with sensors, buttons, LEDs, an LCD display, and serial communication.

One area where I could improve is the organization of the hardware wiring. Although I was able to integrate the components, making the wiring more organized would improve the overall setup and make troubleshooting easier. I also see opportunities to improve the software by refining the organization of the code and making the different components easier to maintain and modify.

Working with hardware has been one of my weaker areas, so this class was particularly valuable in helping me build confidence in that area. I learned more about connecting components, understanding their behavior, and identifying potential problems when hardware and software do not work together as expected.

The problem-solving skills I developed during this project will be useful in future coursework and professional projects. I learned the importance of breaking a complex problem into smaller tasks, testing individual components, and troubleshooting issues systematically. I also focused on using good coding practices to keep the program readable and maintainable. Overall, this project strengthened my programming skills and gave me a better foundation for working with embedded systems in the future.
