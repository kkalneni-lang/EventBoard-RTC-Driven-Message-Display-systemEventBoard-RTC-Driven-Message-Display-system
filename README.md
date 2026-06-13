# EventBoard-RTC-Driven-Message-Display-systemEventBoard-RTC-Driven-Message-Display-system
EventBoard is an embedded systems project developed using the LPC2148 ARM7 microcontroller that automatically displays scheduled messages on a 16x2 LCD based on real-time clock (RTC) events. The system provides secure administrator access for managing schedules and selecting active messages through a keypad-based password authentication mechanism.

# EventBoard - RTC Driven Message Display System

## Overview
EventBoard is an embedded system project built using the **LPC2148 ARM7 microcontroller**. It automatically displays predefined scrolling messages on a **16x2 LCD** at scheduled times using the internal **RTC (Real-Time Clock)**.

The system also provides a secure **Admin Mode**, where authorized users can edit the current time and select active messages using a keypad with password protection.

---

## Features
- RTC-based automatic message display  
- Scrolling text on 16x2 LCD  
- Secure Admin Mode with password  
- Real-time clock display  
- Temperature monitoring using LM35  
- Message scheduling system  
- Green/Red LED status indication  

---

## Hardware Requirements
- LPC2148 Microcontroller  
- 16x2 LCD  
- 4x4 Matrix Keypad  
- LM35 Temperature Sensor  
- LEDs (Green & Red)  
- Switch (Admin Mode)  
- Buzzer  

---

## Software Requirements
- Embedded C  
- Keil uVision  
- Flash Magic  

---

## Working
1. The RTC continuously tracks current time.
2. The system stores **10 predefined messages** in memory.
3. At scheduled times, matching messages are displayed on LCD with scrolling.
4. **Green LED** turns ON when a scheduled message is displayed.
5. If no message is scheduled:
   - Current time is shown
   - Room temperature is displayed
   - **Red LED** turns ON
6. Admin can enter secure mode using switch + password.
7. In Admin Mode, user can:
   - Edit RTC time
   - Enable/Disable messages

---

## Block Diagram
```text
Keypad + Switch + LM35
         |
         v
      LPC2148 + RTC
      /    |    \
     /     |     \
   LCD  Green LED Red LED
```

---

## Applications
- College Notice Boards  
- Event Reminder Systems  
- Smart Scheduling Displays  
- Office Announcement Boards  

---

## Technologies Used
- Embedded C  
- ARM7  
- RTC  
- ADC  
- LCD Interfacing  
- Keypad Interfacing  

---

## Author
**Mallela Vishnu Teja**  
Embedded Systems Developer
