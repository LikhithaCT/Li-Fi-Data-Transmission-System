Li-Fi Data Transmission System

A Li-Fi (Light Fidelity) based wireless data transfer system that uses LED light pulses to transmit text messages, decoded by an LDR sensor and displayed on an LCD screen.

## 📌 Aim

To design and implement a Li-Fi based data transfer system using LEDs and an LDR sensor for wireless, high-speed, and low-cost communication through visible light.

## 🧰 Components Used
-ATmega328 Microcontroller
-Push Buttons
-LDR (Light Dependent Resistor) Sensor
-Regulator Circuitry
-Switches
-LEDs
-breadboard
-Resistors
-Capacitors
-Transistors
-Cables and Connectors
-16x2 LCD Display

##💡 How It Works

Li-Fi (Light Fidelity) is a wireless communication technology that uses visible light from LEDs to transmit data. 
It works on the principle of Optical Wireless Communication (OWC), where data is transmitted through light intensity variations.

An Android app acts as the transmitter, converting text messages into light flashes using the phone's flashlight.
The LDR sensor (receiver) detects these light pulses and converts them into electrical signals.
The ATmega328 microcontroller processes the pulse pattern and decodes the corresponding message.
The decoded message is displayed on a 16x2 LCD screen.

## 🔢 Quantization

Quantization is the process of converting a continuous range of analog values into discrete digital levels.
In this project, it's used in Analog-to-Digital Conversion (ADC) to represent the LDR's analog light intensity readings as digital data the microcontroller can process.

Applications in this system:

-Converts analog light intensity signals from the LDR into digital data
-Helps in accurate data sampling and decoding
-Enables error-free, faster digital communication between transmitter and receiver

##📊 Message Encoding

Messages are encoded as a number of light pulses:

Pulses	Message
1	hi
2	hello
3	how are you?
4	I am fine
5	ok
6	good morning
7	good afternoon
8	good evening
9	thank you
10	sorry

## 📈 Observation Table

| S.No  |	Message Sent (via App) |	Light Detection by LDR |	Decoded Message on LCD |	Result |
|-------|------------------------|-------------------------|-------------------------|---------|
| 1 |	Hi |	Detected |	Hi |	Successful |
| 2	| Hello	| Detected	| Hello	| Successful |
| 3 |	Good Morning |	Detected |	Good Morning |	Successful |
| 4	| Thank you |	Detected |	Thank you	| Successful |

##🚀 Getting Started


Wire the circuit as per the diagram above.
Upload lifi_transmitter_receiver.ino to your ATmega328 using the Arduino IDE.
Open the Serial Monitor at 9600 baud to view debug output.
Use a compatible Li-Fi transmitter Android app to flash messages via your phone's flashlight.
Point the flashlight at the LDR sensor and send a message — it will appear on the LCD.

##👥 Team
Likhitha C T — 1AT24EC417
Sahana A — 1AT24EC425

Guide: Dr. Gayatri Joshi, Assistant Professor, Dept. of ECE

Institution: Atria Institute of Technology, under Visvesvaraya Technological University (VTU), Belagavi

📄 License

This project was developed as part of an academic mini-project submission for the Bachelor of Engineering degree in Electronics and Communication Engineering (2025–26).
