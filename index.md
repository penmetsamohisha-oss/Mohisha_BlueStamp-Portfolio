# Routine Reinforcement Armband
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Mohisha P | Aberdeen High School | Biomedical Engineering | Incoming Sophomore

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**



For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

# First Milestone


<iframe width="560" height="315" src="https://www.youtube.com/embed/2T25-TxnDEk?si=ZgSz9lrB-076J5-b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

My project involves the development of a Routine Reinforcement Armband which is intended to monitor a person's movements, body temperature, and to send alerts via vibration. The Arduino ESP32 functions as the device's central unit by gathering data from the accelerometer, the temperature sensor, and managing the vibration motor. In my first milestone, I tested each of the components individually before putting them all together. To begin with, I connected the ESP32 to my computer and uploaded a program which makes an LED blink in order to check that the device was functioning. Next, I tested the vibration motor by writing a program to switch it on and off, checked the accelerometer by observing how its X, Y ,and Z values changed when the device was moved, and tested the temperature sensor by viewing its readings in the Serial Monitor. A difficulty that I encountered was ensuring that the wiring, the pins, the board settings, and the Arduino libraries were all correct. For my next milestone, I intend to combine the sensors so that an alert is triggered if there is movement detected. Later on, I plan to connect the armband to Wi-Fi, set up a website to show the data it collects, as well as design the complete system into a wearable form.

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
