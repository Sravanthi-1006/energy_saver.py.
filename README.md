📘 Smart Energy Saver – Automation Project
A simple, efficient IoT-inspired smart energy-saving system built using Python automation logic and ECE sensor principles.
This project simulates real-world IoT sensors like LDR (light sensor), PIR (motion sensor), and Temperature Sensors (LM35/DHT11) to automatically control electrical devices and also to decide when to turn electrical devices ON/OFF automatically.

🚀 Project Overview

This Smart Energy Saver helps reduce unnecessary electricity consumption by making intelligent decisions based on:

Light intensity

Temperature

Motion detection

The system uses Python to simulate sensor readings and applies embedded decision logic, similar to what you would implement in an IoT or microcontroller-based system.

🔧 Features

Sensor-based automation

Embedded-style control logic

Low-light detection

Temperature-controlled switching

Occupancy-based power saving

Beginner-friendly

Extendable to real IoT hardware

🧠 Technologies Used

Python

Automation Logic (IF/ELSE)

LDR, PIR, LM35 Sensor Concepts

ECE Embedded Systems Fundamentals

IoT Automation Principles

📂 Project Files
File	Description
energy_saver.py	Main Python automation code
Smart_Energy_Saver_Project_Report.pdf	Full project documentation
screenshot.png	Sample output screenshot (optional)
▶️ How to Run the Project

Install Python (or use online compilers like Replit/JDoodle)

Run the code:

python energy_saver.py


Enter the sensor values when asked:

Light intensity (0–300)

Temperature (°C)

Motion detected (1/0)

🖥️ Code Snippet
print("SMART ENERGY SAVER SYSTEM\n")

light = int(input("Enter light intensity (0-300): "))
temp = int(input("Enter room temperature (°C): "))
motion = int(input("Motion detected? (1 = Yes, 0 = No): "))

if motion == 1:
    if temp > 27:
        print("\nOutput: Turn ON device (Cooling required)")
    elif light < 50:
        print("\nOutput: Turn ON device (Low light detected)")
    else:
        print("\nOutput: Turn OFF device (Conditions normal)")
else:
    print("\nOutput: Turn OFF device (No occupancy detected)")

📊 Sample Output
SMART ENERGY SAVER SYSTEM

Enter light intensity: 80
Enter temperature: 32
Enter motion: 1

Output: Turn ON device (Cooling required)

🔌 How It Works (ECE Explanation)
1. LDR (Light Sensor)

High resistance in low light

If low light + motion → device ON

2. Temperature Sensor (LM35/DHT11)

Outputs temperature

If temperature > 27°C → cooling device ON

3. PIR Sensor

Detects human presence

If no motion → automatic OFF

4. Embedded Logic (Implemented in Python)
if motion == 0 → OFF
if motion == 1 and temp > 27 → ON
if motion == 1 and light < 50 → ON
else → OFF

🏠 Applications

Smart homes

IoT automation

Classroom lighting systems

Office energy management

Industrial automation

✅ Conclusion

This project effectively demonstrates how ECE sensor principles + Python automation can work together to save energy. It is simple, scalable, and can be directly extended into a real-world IoT-based smart home system using Arduino or Raspberry Pi.

📎 Author

Sravanthi
Final-Year ECE Student
Smart Automation & Python Enthusiast
