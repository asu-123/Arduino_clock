# Arduino_clock
A arduino based digital clock simulation.
# Arduino-Based Clock Simulation

This project demonstrates a clock simulation using Arduino and a 4-digit 7-segment display to show minutes and seconds. The system is designed efficiently to use only 11 Arduino pins instead of the 29 pins typically required by 4 displays. This is achieved through time segmentation to drive all 4 displays simultaneously.

---

## Features

- **4-Digit Clock Display**: Shows minutes and seconds in real-time.
- **Efficient Pin Usage**: Utilizes only 11 pins of the Arduino.
- **Time Segmentation**: Implements multiplexing to control all 4 displays simultaneously.

---

## Components Used

1. **Arduino Uno**
2. **4-Digit 7-Segment Display**
3. **Resistors**
4. **Breadboard**
5. **Jumper Wires**

---

## Circuit Diagram

Refer to the image included in this repository for the circuit diagram. Ensure to double-check all connections before powering the system.

---

## Code

The Arduino code (`clock_simulation.ino`) handles:

- Multiplexing logic to drive 4 displays using 11 pins.
- Timekeeping to update the display in real-time.

---

## How It Works

1. **Multiplexing**: The code divides time into segments, activating one display at a time at a high frequency. This gives the illusion that all displays are on simultaneously.
2. **Time Tracking**: Internal counters keep track of seconds and minutes.
3. **Display Update**: Each segment of the display is refreshed based on the time values.

---

## Setup Instructions

1. Assemble the circuit as shown in the provided diagram.
2. Connect the Arduino to your computer using a USB cable.
3. Upload the `clock_simulation.ino` code to the Arduino using the Arduino IDE.
4. Power the Arduino to start the clock.

---

## Future Enhancements

- Add an RTC (Real-Time Clock) module for accurate timekeeping.
- Include buttons to set the time manually.
- Add an alarm feature with a buzzer.
- Hour segment will be added
---

## License

This project is open-source and available under the MIT License. Feel free to use and adapt it for your needs.

---

## Contribution

Contributions are welcome! Open an issue or submit a pull request with your improvements or suggestions.

