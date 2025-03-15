<img width="258" alt="image" src="https://github.com/user-attachments/assets/f155da63-79d0-42f8-b600-c99c956a502c" />

Group 1: Su Wai Phyoe, Wang Qin, Lu Liu 
<Heartie>
User Manual


First Year Hardware Project/br
School of ICT
Metropolia University of Applied Sciences
14.3.2025 
Version history 
 
Ver 	Description 	Date 	Author(s) 
1.0	Wrote introduction and getting started parts for user manual 	13.3.2025	Su Wai Phyoe

	Wrote using the device part for user manual 	13.3.2025	Wang Qin
	Wrote troubleshooting and additional information for user manual	14.3.2025	Su Wai Phyoe, Wang Qin
			
			
  	  	  	  
  	  	  	  
  	  	  	  
  	  	  	  
 
Contents
1	Introduction	1
Glossary	1
2	Getting Started	2
Hardware Assembly	2
3	Using the Device	3
3.1	How does Heartie work	3
3.2	How to Interpret the Results	4
4	Troubleshooting	6
5	Additional information	6
5.1	Contact Information	6
5.2	Technical Specification	7
5.3	Feedback form	7
5.4	Self-Repairing	7
5.5	Device Properties	7

 
1	Introduction
Welcome to the user manual of “Heartie” heart rate detector. This innovative device allows users to accurately measure pulse rate and heart rate variability. Whether you're a medical professional monitoring patient health, a fitness enthusiast tracking your performance, or a researcher collecting data, this device is designed to provide reliable results in real-time. This manual will guide you through the setup process, explain how to operate Heartie, and offer solutions for common issues you might encounter.
Intended Users

●	Medical Professionals
●	Athletes & Fitness Enthusiasts
●	General Users
Glossary
Parameter	Unit	Description
SDNN	ms	Standard deviation of NN intervals
SDRR	ms	Standard deviation of RR intervals
SDANN	ms	Standard deviation of the average NN intervals for each 5 min segment of a 24 h HRV recording
SDNN index	ms	Mean of the standard deviations of all the NN intervals for each 5 min segment of a 24 h HRV recording
pNN50	%	Percentage of successive RR intervals that differ by more than 50 ms
HR Max – HR Min	bpm	Average difference between the highest and lowest heart rates during each respiratory cycle
RMSSD	ms	Root mean square of successive RR interval differences
HRV triangular index		Integral of the density of the RR interval histogram divided by its height
TINN	ms	Baseline width of the RR interval histogram
2	Getting Started
Hardware Assembly
To get Raspberry Pi Pico and Pulse Sensor up and running, follow these steps:
1.	Connect the sensor's wires properly: The red wire goes to the 3.3V power pin, the black wire to ground (GND), and the yellow wire to the signal pin on the Raspberry Pi Pico.
2.	Secure the setup: Place the Raspberry Pi Pico on a breadboard to keep the connections stable and organized.
3.	Establish the power source: Connect the Raspberry Pi Pico to computer via a USB cable. This will provide both power and allow data transfer.
●	Powering On: Connect the Raspberry Pi Pico to the USB cable, which will automatically power on the device and start the pulse monitoring script.
●	Place the finger on the sensor: Allow the optical detector to pick up your pulse.
●	Monitor the data: Watch the OLED display for continuous updates.
●	Powering Off: Disconnect the USB cable to turn off the device.
●	Ensure stability: Place the device on a steady surface to avoid external interference.
3	Using the Device
Your pulse and heart rate are two different ways to track your heart’s activity. Your heart rate is how many times your heart beats per minute. Your pulse rate is how many times per minute your arteries expand because of your heart beating. There’s usually no difference between your heart rate and your pulse rate (or the difference is very small). 
3.1	How does Heartie work
Optical (photoplethysmography): Heartie uses infrared light to see the expansion of your arteries as your heart pumps blood through them. Heartie tracks your pulse rate, and some can also estimate the oxygen levels in your blood. It also measures and displays other metrics, like heart rate variability.

 
 
  

3.2	How to Interpret the Results
Heartie displays your heart rate in beats per minute (BPM).
●	Normal Resting Heart Rate: A normal resting heart rate for adults typically ranges from 50 - 70 BPM.
 
 
●	Heart Rate Zones: Heartie displays different heart rate zones: recovery/easy, aerobic/base, tempo, lactate threshold, anaerobic. Each zone indicates a different level of intensity.
 
●	Abnormal Readings: If you consistently observe readings outside the normal range, or experience any discomfort, consult your doctor.



  Additional Tips:
●	Cleaning: Clean the device regularly with a soft cloth. 
●	Accuracy: The accuracy of the readings may vary depending on factors such as skin contact, body position, and movement.
●	Storage: Store the device in a cool, dry place.
  Safety Precautions
●	Do not use the device while operating machinery or driving.
●	Do not immerse the device in water.
●	Avoid direct sunlight on the sensor. This can interfere with the readings
●	Use in a stable environment. Avoid excessive hand movement for accurate readings.
●	This device is not a medical device and should not be used to diagnose or treat medical conditions. Consult a healthcare professional for any health concerns.
4	Troubleshooting
1.	Inconsistent Readings: Keep your finger still on the sensor and ensure proper positioning.
2.	No power or data transfer: Verify that the USB cable is properly connected to the Raspberry Pi Pico and the computer. Check for any loose wiring on the breadboard.
3.	Signal pin issues: Ensure the yellow signal wire is correctly connected to the designated pin on the Raspberry Pi Pico.
5	Additional information
5.1	Contact Information
Email address: customerservice.group1@metropolia.fi
mobile: +358457416677
visit at Karaportti 2, 02610 Espoo,Finland
5.2	Technical Specification
          Battery type: 2 AA batteries
         Memory Capacity: 4GB,
         Screen Resolution:128×64,
         Maximum Power: 15.3W USB-C Power Supply,
         Wi-Fi Frequency: 2.4GHz Wi-Fi
5.3	Feedback form
We are happy to hear your feedback:
https://docs.google.com/forms/d/e/1FAIpQLScT6i8O6Pr-r1IqVbxTfe_lokrmwKqh5-csxHVobN3QdUATFQ/viewform?usp=dialog
5.4	Self-Repairing
1.    Choose platform: Install MicroPython.
2.    Get the right libraries: Download the necessary libraries for pulse detection and OLED display management.
3.    Upload the script: Using an IDE like Thonny, upload the pulse monitoring script to the Raspberry Pi Pico.
4. Click “run current script”
5.5	Device Properties
Raspberry Pi 4 Model B(4GB version): 2.4 GHz and 5.0 GHz IEEE 802.11ac
wireless, Bluetooth 5.0, BLE Gigabit Ethernet, 2 USB 3.0 ports, 2 USB 2.0
ports, 2 × micro-HDMI® ports (up to 4kp60 supported), Micro-SD card slot.For detailed technical information visit: Raspberry Pi 4 Model B specifications.

Raspberry Pi Pico W: Dimensions 15 cm × 10 cm × 5 cm, Weight: 350g,
Wireless (802.11n), single-band (2.4 GHz), Bluetooth 5.2. For detailed technical
information, please visit: Raspberry Pi Pico W datasheet
![image](https://github.com/user-attachments/assets/bebbaf47-09ee-4f46-aafc-bcbd0e6ecee6)

---
