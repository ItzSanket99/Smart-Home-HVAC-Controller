# KPIT_Honors_Assessment
<img width="1192" height="655" alt="Hardware Setup" src="https://github.com/user-attachments/assets/0dc82646-382a-4fe3-b580-50ef36883350" />

Repository for the project assessment of the Honors Course – KPIT Apex Lab (EP & ACN).
This project demonstrates real-time embedded system design using STM32, FreeRTOS, and temperature monitoring (LM35) as part of the Honors curriculum.

## 🖼️ Project Overview

## 🚀 Smart Home HVAC Controller – STM32 + FreeRTOS

This embedded system monitors temperature in real time using an LM35 sensor and performs HVAC control tasks using FreeRTOS concepts such as multitasking, queues, mutex protection, and tickless idle low-power mode.

The project highlights RTOS-based task structuring, resource management, and efficient peripheral usage on STM32.

## ⭐ Key Features

✔️ Real-time temperature sensing using ADC

✔️ Multi-tasking using FreeRTOS

✔️ Queue-based inter-task communication

✔️ UART output with mutex protection

✔️ Tickless idle mode (power saving)

✔️ Modular task design: Sensor Task, Control Task, UART Task

## 🧱 System Architecture
RTOS Tasks
Task	Description
Sensor Task	Reads LM35 via ADC, converts analog value to temperature
Control Task	Implements basic HVAC logic (cooling ON/OFF)
UART Task	Logs system status securely using mutex

## Peripherals Used
- **ADC1** – Temperature sensing  
- **UART2** – System logs  
- **GPIO** – Status indicators  
- **SysTick** – RTOS scheduler  


## 🔌 Hardware Setup

| Component   | STM32 Pin     |
|-------------|---------------|
| LM35 Output | PA1 (ADC1_IN1) |
| LM35 VCC    | 5V            |
| LM35 GND    | GND           |
| UART TX     | PA2           |
| UART RX     | PA3           |


## 📂 Folder Structure

KPIT_Honors_Assessment/
│
├── Core/
│   ├── Inc/
│   ├── Src/
│
├── Drivers/
│   ├── CMSIS/
│   └── STM32F4xx_HAL_Driver/
│
├── README.md
└── .project files


## 🧠 Concepts Learned
- Embedded C programming  
- STM32 peripheral configuration (ADC, UART, GPIO)  
- FreeRTOS concepts:  
  - Tasks  
  - Queues  
  - Mutexes  
  - Tickless idle  
- Debugging using STM32CubeIDE  
- Real-time task synchronization  
- Inter-task communication  


## ▶️ How to Run
1. Clone the repository  
2. Open the project in **STM32CubeIDE**  
3. Build the project  
4. Flash to STM32F446RE board  
5. Open UART Terminal @ **115200 baud**  


## 🤝 Team
- **Sanket Jagtap**  
- **Rachana Mahangare**  
- **Anjali Bhamare**  

