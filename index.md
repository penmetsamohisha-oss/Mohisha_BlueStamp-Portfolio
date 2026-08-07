# Routine Reinforcement Armband
This project features an armband that uses an Arduino Nano ESP32 to perform routine correspondence by monitoring an individual's movement and temperature while giving instructions through a buzzer and vibration motor. Moreover, I added various sensors, such as a flex sensor to measure arm bending, a heart-rate detector to measure beats per minute, and an OLED display to show all measurements on the device. Additional improvements involve rearranging the components on two breadboards linked together, which makes the armband feasible to wear. Finally, I designed a website to display live readings, alert conditions, and heart-rate and movement graphs by connecting to the controllers via Bluetooth Low Energy. 

| Mohisha P | Aberdeen High School | Biomedical Engineering | Incoming Sophomore |
![Routine Reinforcement Armband](routine-armband.jpg)

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

# Final Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug](https://www.youtube.com/watch?v=qgViM-uNFv4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

After my last milestone, I have made several changes to the Routine Reinforcement Armband. I divided the circuit among two breadboards, added a flex sensor, heart-rate sensor, and OLED display, and created a website to collect real-time sensor data through Bluetooth Low Energy.


The most difficult part was making sure that all parts would work together properly. I had many problems troubleshooting wiring, sensor connections, the power supply, and Bluetooth communication. I consider my biggest achievement to be integrating the hardware, Arduino programming, Bluetooth connectivity, and the website into one working system.


While working on the BSE project, I learned more about circuit design, Arduino programming, connecting analog and digital sensors, and debugging. I also learned about Bluetooth Low Energy services and characteristics and how they can be used to send sensor data wirelessly.


In the future, I would like to make the armband smaller and more “wearable” by replacing the breadboards with a permanent circuit, adding a battery charger, improving sensor accuracy, and creating a better website that can store and analyze the data over time. 




# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**
<iframe width="560" height="315" src="https://www.youtube.com/embed/2T25-TxnDEk?si=ZgSz9lrB-076J5-b](https://www.youtube.com/watch?v=tu1wzGVcvsc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Ever since I achieved my initial milestone, I have dedicated my time and efforts to completing the foundation of my Routine Reinforcement Armband. I wired and programmed the main components of the armband, namely the MPU6050 movement sensor, TMP36 temperature sensor, buzzer, vibration motor, and mute button. Not only did I implement the wiring, but I also made sure that the armband is able to calibrate and set alert thresholds, which allow it to detect movement and temperature variations.

Perhaps one of the most unexpected aspects of this stage was the technical difficulties I had to overcome to achieve smooth, correct functioning of all components at the same time. It turned out that I had to troubleshoot wiring, check the performance of each individual sensor, calibrate thresholds, and check the efficiency of the motor and buzzer.


Combining sensors and outputs to operate together in a single system was one of the toughest challenges faced at this stage. Each element was capable of working independently, but connecting the different elements required changing the wiring and coding to ensure simultaneous operation without any conflicts. 

In the future, I still have to make the armband more wearable, together with all the modifications to my idea.

# First Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/2T25-TxnDEk?si=ZgSz9lrB-076J5-b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

My project involves the development of a Routine Reinforcement Armband which is intended to monitor a person's movements, body temperature, and to send alerts via vibration. The Arduino ESP32 functions as the device's central unit by gathering data from the accelerometer, the temperature sensor, and managing the vibration motor. In my first milestone, I tested each of the components individually before putting them all together. 

To begin with, I connected the ESP32 to my computer and uploaded a program which makes an LED blink in order to check that the device was functioning. Next, I tested the vibration motor by writing a program to switch it on and off, checked the accelerometer by observing how its X, Y ,and Z values changed when the device was moved, and tested the temperature sensor by viewing its readings in the Serial Monitor. 

A difficulty that I encountered was ensuring that the wiring, the pins, the board settings, and the Arduino libraries were all correct. For my next milestone, I intend to combine the sensors so that an alert is triggered if there is movement detected. Later on, I plan to connect the armband to Wi-Fi, set up a website to show the data it collects, as well as design the complete system into a wearable form.

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials

| **Part** | **Note** | **Price** | **Link** |
| :--- | :--- | :--- | :--- |
| Arduino ESP32 | The essential microcontroller of the band. It collects data from the pressure, movement, and temperature sensors and activates the vibration motor when required. | $20.00 | [Link](https://www.amazon.com/dp/B0C947BHK5) |
| Resistive Force Sensor | Detects pressure when the user presses or squeezes it. It can serve as an input to confirm a notification, cancel an alarm, or communicate with the band. | $11.99 | [Link](https://www.amazon.com/dp/B0CZ6L5NMM) |
| Vibrating Mini Motor | Creates vibrations that can be felt on the arm. It provides silent notifications when movement or an unusual temperature is detected. | $5.99 | [Link](https://www.amazon.com/dp/B0DY65KVQR) |
| Accelerometer | Detects the movement, acceleration, and orientation of the arm. The ESP32 compares its readings with the arm’s starting position and activates a warning when the movement threshold is exceeded. | $11.25 | [Link](https://www.amazon.com/dp/B0D2TJVMNY) |
| USB-C Cable | Connects the ESP32 to a computer. It is used to upload the Arduino program, monitor sensor readings, troubleshoot the system, and power the prototype. | $3.88 | [Link](https://www.amazon.com/dp/B01GGKYKQM) |
| Analog Temperature Sensor | Reads the temperature close to the user’s skin and sends an analog voltage to the ESP32. The program can alert the user when the temperature is outside the selected safe range. | $12.00 | [Link](https://www.amazon.com/dp/B0GKG3FLCL) |
| Armband | Keeps the sensors, vibration motor, and electronic components secure on the user’s arm. It makes the device portable and allows the user to feel the vibrations clearly. | $5.50 | [Link](https://www.amazon.com/dp/B0D58Z7KMK) |
| Electronics Kit | Includes a breadboard, jumper wires, resistors, and other small components needed to connect and test the circuit. These parts are useful for building and debugging the prototype. | $14.00 | [Link](https://www.amazon.com/dp/B0B62RL725) |
| 9V Barrel Jack | Connects the 9V battery to the prototype’s power circuit. It allows the project to be tested without remaining connected to a computer. | $6.00 | [Link](https://www.amazon.com/dp/B07FDS11ZY) |
| Digital Multimeter | Measures voltage, resistance, and electrical continuity. It helps check battery voltage, test connections, and locate damaged or disconnected wires. | $9.99 | [Link](https://www.amazon.com/dp/B0CXM242J1) |
| 9V Batteries | Provide a portable power supply for the project during testing. A suitable voltage regulator must be used before powering the ESP32. | $12.37 | [Link](https://www.amazon.com/dp/B00MH4QM1S) |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
