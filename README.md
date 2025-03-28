# Programmable Logic Controllers: Milk Pasteurization Automation

## 🌡️ What is Pasteurization?  
Pasteurization is a heat-treatment process used to destroy harmful microorganisms in certain foods and beverages. It was developed by French scientist Louis Pasteur in the 1860s, who discovered that heating wine and beer to around 57°C (135°F) for a few minutes could prevent abnormal fermentation caused by microbes.  

Today, pasteurization is widely used in the dairy industry to ensure the safety and shelf life of milk. The two most common methods are:  

High-Temperature Short-Time (HTST): Milk is heated to approximately 72°C (161°F) for 15 seconds, then rapidly cooled.  

Ultra-High Temperature (UHT): Milk is heated to about 135°C (275°F) for a few seconds, allowing it to be stored without refrigeration until opened.  

This project focuses on automating the HTST pasteurization process using a PLC-based control system.  

## ⚙️ Project Overview  
This automation system was designed using Programmable Logic Controllers (PLCs) to simulate and control the milk pasteurization process. It includes temperature monitoring, timing control, and safety checks — all visualized through a Human-Machine Interface (HMI).  

## 🔁 Pasteurization Workflow  
Below is the complete pasteurization process implemented in the system:  

![image](https://github.com/user-attachments/assets/edc3b3b5-93ce-42dd-b7c0-c93a7c009f03)


## 🖥️ HMI Screens
Screens designed for the Human-Machine Interface (HMI) to monitor and control the pasteurization process:

## 🚀 1. Navigation Interface
![image](https://github.com/user-attachments/assets/1dab1fb1-a151-419d-8618-8170fda3080d)

A central navigation panel provides quick access to processes:  
Raw Milk Tank  
Heat Exchange  
Cooling  
Pasteurized Milk  
Log Off  

## 🔐 2. Login Interface
Before interacting with the system, the operator must log in with a username and password. This ensures that only authorized personnel can access or modify critical operations. Once logged in, the operator can access the wanted panel.   
![image](https://github.com/user-attachments/assets/8c82bb02-2db5-4e3b-9ac3-3ab4cc2a0d87)

## 🥛 3. Raw Milk Tank Screen and 🧪 Fat Separation
The process begins with raw milk storage in a balance tank. This tank ensures a continuous and stable flow of milk into the pasteurization system. Operators monitor the tank level here and ensure that the supply is ready for processing. This step prepares the milk for pre-heating and ensures homogenization.

It allows operators to manage the filling and draining of a separator tank. A mixer is controlled from the panel, and the desired fat percentage can be set.
This step allows for standardizing the fat content of the milk, depending on the end product.  

https://github.com/user-attachments/assets/c58f5c3b-605d-4dd0-94bf-9be0b93b1bc0

## ♨️ 4. Heat Exchange – Pasteurization Phase
After raw milk enters the system, it moves through a heat exchanger. Using hot water or steam, the system raises the milk temperature to 72°C, the required level for High-Temperature Short-Time (HTST) pasteurization.

The operator sets the initial and target temperatures directly from the screen. Once the start button is pressed, the system begins heating, and a live graph displays the temperature progression over time, ensuring that milk reaches and holds the desired level for the necessary duration (at least 15 seconds).

https://github.com/user-attachments/assets/710ca6c6-e729-4175-a49e-072f51afc0e2


## ❄️ 5. Cooling Phase
After pasteurization, the milk must be rapidly cooled to prevent bacterial growth and preserve freshness. The milk flows through a cooling section where its temperature is brought down to around 4°C using chilled water.

The HMI screen allows the operator to set the output temperature and monitor the cooling curve in real time. Similar to the heating phase, a graph on the screen tracks the temperature drop, confirming proper cooling.

https://github.com/user-attachments/assets/a0d20c31-27ff-45fb-be24-de6363672697


## 🍼 6. Bottling & Final Storage
Once the milk has been pasteurized and cooled, it is transferred to a storage tank for bottling. The system displays the current tank level and keeps track of the number of bottles being filled.

When the Bottle button is pressed, the filling operation begins, and the bottle count increases in real time. A high-level alert is shown on the screen when the tank is near capacity, helping operators avoid overflows.

https://github.com/user-attachments/assets/a2f4e05f-75fb-4f44-be71-78303a1fc6d6
https://github.com/user-attachments/assets/8dcce27c-2110-4e41-bc2a-a8cbd92d6315


## 🚀 Technologies Used
PLC Programming: Ladder Logic with Siemens TIA Portal
HMI Software: WinCC  
Simulation Tools: PLCSIM  

