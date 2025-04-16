# IoT-Based-Weather-Monitoring-System
## Introduction
In today’s world, real-time environmental monitoring is crucial for both daily life and long-term sustainability. With the growing impact of climate change and air pollution, accurate weather data collection has become more important than ever. The “IoT-Based Weather Monitoring System” is a smart solution that collects temperature, humidity, and air quality data using sensors, then transmits this data to a mobile-based cloud dashboard using IoT technology. Our project uses the NodeMCU ESP8266 Type-C version as the microcontroller, along with a DHT11 sensor for temperature and humidity and an MQ-135 gas sensor for air quality. These components work together to provide live environmental readings, which are displayed through the IoT Remote App. 
## Motivation
As students of Embedded Systems and IoT, we wanted to build a project that not only uses real-time data collection but also has real-world applications. Weather conditions affect our daily activities, agriculture, health, and safety. However, many local areas still lack affordable and reliable monitoring systems. This inspired us to develop a simple, low-cost, and effective weather monitoring system that can be used in homes, schools, farms, or any remote location with internet access. 
## Objectives
The main objectives of this project are:

•	To collect real-time temperature, humidity, and air quality data using sensors.

•	To transmit this data wirelessly to a cloud-based platform using the NodeMCU.

•	To display the collected data in a user-friendly way on a mobile app (IoT Remote App).

•	To design a scalable and cost-effective prototype for future development or deployment.

## Feasibility Study
From a technical perspective, this project is highly feasible as it uses readily available components and open-source platforms. The NodeMCU ESP8266 is a Wi-Fi-enabled microcontroller that allows easy internet connectivity. Sensors like DHT11 and MQ-135 are low-cost and compatible with most microcontrollers. The use of the IoT Remote App simplifies the data visualization process without needing complex server setup. From a financial standpoint, the entire project is budget-friendly and suitable for academic and small-scale commercial use.
## Gap Analysis
Traditional weather monitoring systems are often large-scale, expensive, and not accessible to individuals or small communities. Moreover, many low-cost solutions lack the ability to provide real-time data or remote access. Our project fills this gap by offering a compact and affordable solution that provides live updates via cloud and mobile technology, making it ideal for rural or remote environments.
## Project Outcome
By the end of this IoT-Based Weather Monitoring System project, we successfully created a functional prototype that collects temperature, humidity, and air quality level data in real time and displays it on a mobile app. The system is easy to set up and can be expanded with more sensors or integrated with other IoT platforms in the future. This project gave us practical experience in working with embedded systems, sensors, and cloud-based IoT applications.

## Overview
Before building the system, we carefully analyzed the basic requirements to make sure our project would be functional, reliable, and user-friendly. The primary goal was to develop an IoT-based weather monitoring system that can collect real-time environmental data and display it on a cloud-connected mobile app. We decided on components that are both cost-effective and suitable for student-level projects, while still offering room for future improvements and scalability.

## Circuit Diagram 
![image](https://github.com/user-attachments/assets/876cd80c-847b-48df-8983-112343d8b711)
Figure: Weather Monitoring Circuit

 ## Dashboard Design
![image](https://github.com/user-attachments/assets/ff5f2830-25b6-4f1c-82c7-b83a545755e0)
![image](https://github.com/user-attachments/assets/c815f4eb-8677-486c-ba35-c1aeefef93e2)

## Overall Project Plan
We divided our project into clear steps to manage tasks efficiently and complete everything on time. The plan followed a simple development lifecycle:

•	Step 1: Requirements gathering and selecting suitable sensors and modules

•	Step 2: Designing the circuit on a breadboard and verifying sensor output

•	Step 3: Programming the NodeMCU using Arduino IDE to read data and send it to the cloud

•	Step 4: Setting up the IoT Remote App for real-time data visualization

•	Step 5: Testing and validating the system performance

•	Step 6: Final adjustments and preparing documentation and presentation

By following this structured plan, we ensured that the system was built systematically, tested properly, and delivered with all necessary documentation.

## Implementation
The implementation phase began with assembling all the necessary components on a breadboard. The NodeMCU ESP8266 was chosen as the microcontroller for its built-in Wi-Fi capabilities, which allowed us to connect to the internet without needing extra modules. We connected the DHT11 sensor for temperature and humidity readings and the MQ-135 gas sensor for air quality monitoring. Jumper cables and a Type-C USB cable were used to power and link all the components.

The NodeMCU was programmed using the Arduino IDE. We used libraries such as “DHT.h” for reading values from the DHT11 sensor and standard analog read functions to gather data from the MQ-135. After collecting sensor values, the data was transmitted over Wi-Fi to the IoT Remote App, which we configured with virtual display widgets for each environmental parameter.

We went through several test runs to ensure that the sensors were correctly sending accurate values and the app was receiving real-time updates. All readings were displayed live on our mobile devices through the IoT Remote platform, making it easy to monitor environmental changes at any moment.

## Performance Analysis
During the testing phase, the system performed consistently within our expectations. The DHT11 sensor delivered stable readings with minor fluctuations, which is normal for this type of sensor. The MQ-135 gas sensor took a few minutes to warm up before giving stable outputs, which we accounted for in our code by delaying data transmission during the initial phase.

The NodeMCU had no problem handling the data collection and transmission simultaneously. Thanks to its onboard Wi-Fi module, we were able to maintain a stable connection with the cloud through the IoT Remote App. Data updates occurred every few seconds, providing near real-time monitoring.

## Key observations:

•	Temperature and humidity readings updated accurately every 2–3 seconds.

•	Gas sensor readings fluctuated slightly depending on air quality and ventilation.

•	The app interface remained responsive and easy to use throughout the test sessions.

•	Power consumption was minimal and could be further reduced with sleep mode features if needed.

## Results and Discussion
Overall, the implementation of our IoT-Based Weather Monitoring System was successful. The system was able to:

•	Collect real-time temperature, humidity, and air quality data

•	Send the collected data to the IoT Remote App using Wi-Fi

•	Display the information in a user-friendly mobile interface

We also tested the system under different environmental conditions, such as placing it in a closed room, near a window, and outdoors. In each case, the readings changed according to the environment, confirming the sensors were working properly.

The main advantage of this system is its simplicity and portability. Anyone with basic technical knowledge can assemble and use it for home, school, or small-scale agricultural purposes. The biggest limitation is the sensor accuracy—while good for learning and basic use, more accurate sensors would be required for professional applications.

## Summary
In this project, we successfully developed an IoT-based weather monitoring system using NodeMCU ESP8266, DHT11 sensor, and MQ-135 gas sensor. The system was able to collect real-time data on temperature, humidity, and air quality, and send that information to a mobile cloud dashboard using the IoT Remote App. Through this project, we not only applied our theoretical knowledge of embedded systems and IoT but also gained valuable hands-on experience in hardware integration, sensor communication, and wireless data transmission.

Our system was able to perform reliably during testing. It provided consistent readings and displayed them in a user-friendly mobile interface, making environmental monitoring more accessible. This project also gave us an opportunity to improve our teamwork, problem-solving, and project management skills.

## Limitation
While the project met its main objectives, there were a few limitations:

•	The DHT11 sensor provides only basic accuracy, and its response time is relatively slow compared to more advanced sensors.

•	The MQ-135 gas sensor can detect a wide range of gases, but it lacks specificity and sometimes shows slight variations depending on surrounding conditions.

•	The system requires a stable internet connection to transmit data to the mobile app, which limits its use in offline or remote areas without Wi-Fi.

•	Power was supplied via USB; for outdoor or long-term use, a battery or solar-powered version would be more practical.

These limitations are common in low-cost prototypes and can be addressed in future versions.

## Future Work
To improve and expand our project, we plan to work on the following enhancements:

•	Replace the DHT11 sensor with more accurate alternatives like DHT22 or BME280 for better temperature, humidity, and pressure readings.

•	Calibrate the MQ-135 sensor more precisely or replace it with specialized air quality sensors to detect specific gases like CO2 or smoke.

•	Integrate battery power or solar charging for portability and long-term deployment.

•	Add a local display module (like an LCD) to show sensor data even without internet connectivity.

•	Implement data logging features so the system can store environmental trends over time, which would be useful for analysis.

•	Introduce alert systems (e.g., push notifications or LED indicators) to warn users of unhealthy environmental conditions.

By making these improvements, we can turn this basic monitoring system into a more robust and reliable solution suitable for a wider range of real-life applications.

