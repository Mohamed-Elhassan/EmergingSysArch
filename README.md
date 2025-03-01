# EmergingSysArch

### Project Summary and Problem Solved
This project implements a thermostat system with three states: off, heat, and cool. The thermostat uses buttons to cycle through the states and adjust the set temperature. The red and blue LEDs represent the heating and cooling states, respectively. If the temperature falls below the setpoint, the red LED pulses; if it exceeds the setpoint, the blue LED pulses. The system also updates a 16x2 LCD to display the current time, temperature, and state of the thermostat. Additionally, it sends status updates every 30 seconds over serial communication to a server, providing real-time information about the thermostat’s state.

### What I Did Particularly Well
I feel good about how the project came together in terms of its functionality. The state machine works smoothly, toggling between heat, cool, and off states. The button interactions for cycling through the states and adjusting the setpoint are intuitive. I also feel the integration with the serial communication is solid and allows for easy status updates, which could be useful for remote monitoring.

### Where I Could Improve
One area I could improve is optimizing the timing for state transitions. Right now, the time management works but could be refined for efficiency. Another improvement could be simplifying the logic for managing the LCD display updates; it works, but there might be a cleaner way to handle alternating lines for display updates.

### Tools and Resources Added to My Support Network
The primary tools I used include the statemachine library to handle state transitions, gpiozero for controlling buttons and LEDs, and the adafruit_character_lcd library for the LCD screen. I also learned how to integrate serial communication with pyserial to send updates. I’ll continue to use these tools in future projects, especially for hardware-related work, and I’ll keep exploring libraries like threading to handle multitasking.

### Transferable Skills from This Project
The experience from this project will definitely help with other embedded systems or IoT projects. Skills like managing hardware components, using state machines for logic, and working with serial communication are directly transferable. I also learned how to handle real-time data processing, which is something that can be applied in other areas like automation or monitoring systems.

### How I Made This Project Maintainable, Readable, and Adaptable
To ensure the project is maintainable, I structured it with clear class definitions for different components, such as the ManagedDisplay and TemperatureMachine. This makes it easier to update individual parts of the system without affecting the entire program. Additionally, I used descriptive variable names and kept the state transitions clear, which enhances readability. I also modularized the functionality (e.g., serial communication, button interactions, and LED state changes), which will make adapting or extending the project easier in the future.
