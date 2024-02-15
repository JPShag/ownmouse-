My attempt at creating a programmable gaming mouse.

1x Teensy board - aquired
Optical Mouse Sensor: Choose a sensor compatible with your Teensy board, such as the ADNS-9800, which offers good performance for DIY mouse projects.
Buttons: For the left and right clicks, and any additional buttons you want for extra functionalities like a middle click, DPI adjustment, or forward/backward.
Optional Components: Depending on your design, you might want additional components like a scroll wheel, LEDs for status indicators, or a surface for the sensor to track movements accurately.


Steps:
1. Design the Circuit:
Connect the optical mouse sensor to the Teensy using its SPI or I2C interface, depending on the sensor's specifications.
Connect the buttons to the Teensy's digital I/O pins. You might need to use pull-up or pull-down resistors to ensure stable button states.
If you're including a scroll wheel, it typically involves a rotary encoder. Connect it to two digital I/O pins for the rotational detection and one for the click function.
For a more stable and professional setup, consider designing a PCB that integrates all these components, or you can start with a breadboard for prototyping.
2. Program the Teensy:
Use the Teensyduino add-on for the Arduino IDE, which provides libraries and tools specifically for programming Teensy boards.
Write your program to read data from the optical sensor and convert it into mouse movements. The Mouse.h library available in Teensyduino can be used to emulate a USB mouse easily.
Implement code to read button presses and translate them into mouse clicks. Use debouncing techniques in your code to ensure reliable button press detection.
If you've included a scroll wheel, write code to read the rotary encoder movements and send them as scroll actions.
Test and refine your code to ensure accurate and responsive mouse movement and button clicks.
3. Assemble the Hardware:
Once your circuit design is finalized and your code is working with your prototype setup, assemble your components. If you've designed a PCB, get it manufactured and solder your components onto it.
Secure the Teensy, sensor, buttons, and any other components inside a mouse casing. You can design and 3D print a custom casing, modify an existing mouse casing, or even build one from scratch using materials like acrylic.
