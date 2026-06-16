# Arduino Binary Calculator System

**Arduino-Based Binary Calculator with Python GUI Integration**

> Developed by *Sara Ghazavi*
> Sharif University of Technology – Winter 1403

---

## 📝 Description

This project was developed as a course assignment for *Computer Language and Structure* at Sharif University of Technology. It implements an **Arduino-based binary calculator system** integrated with a Python GUI application through serial communication.

The system simulates a microcontroller-based computational unit with keypad input and LCD output. The firmware runs in the Wokwi simulation environment, while a Python desktop application communicates with the Arduino via a serial protocol to provide a graphical interface for user interaction.

The project demonstrates fundamental concepts of I/O interfacing, embedded control logic, and hardware-software integration. The design emphasizes modular firmware architecture and structured communication between embedded and host systems.

---

## 📁 Features

### ✅ Embedded System (Arduino)

* Keypad-based binary input system
* LCD output display using I2C interface
* Stack-based binary arithmetic operations
* Structured control logic for parsing and execution
* Designed for Wokwi simulation environment

### ✅ Python GUI Application

* Graphical user interface built with Tkinter
* Serial communication with Arduino firmware
* Real-time interaction and result visualization
* External control of the embedded system

---

## 🛠️ Technical Stack

* **Microcontroller Platform**: Arduino
* **Language (Embedded)**: C++ (Arduino)
* **Language (Desktop App)**: Python
* **GUI Framework**: Tkinter
* **Communication**: Serial Protocol (RFC2217)
* **Simulation Environment**: Wokwi
* **I/O Components**: Keypad, LCD (I2C)

---

## 📘 Educational Objectives

* Understand microcontroller-based system design
* Implement I/O interfacing (keypad and LCD)
* Design structured, state-driven control logic in embedded firmware
* Implement serial communication between the host and the device
* Explore hardware-software co-design principles

---

## 🚀 Getting Started

### Running the Arduino Simulator
To run the **binary calculator** in the Wokwi simulator:

1. Install the **Wokwi Extension** in Visual Studio Code.
2. Open `sketch.ino` located in the `./sketch` directory.
3. Press `Ctrl + Shift + P` and search for **"Wokwi"**.
4. Click on **"Wokwi: Start Simulator"**.

### Running the Python GUI Application
To run the **Python-based GUI**:

1. Ensure you have Python installed on your system.
2. Install required libraries (if not installed):
   ```sh
   pip install pyserial tkinter
   ```
3. Run the application:
   ```sh
   python app.py
   ```

---

## 📜 Dependencies

### ➤ Libraries Used in the Arduino Simulator:
- `<ArduinoQueue.h>`
- `<LiquidCrystal_I2C.h>`
- `<SimpleStack.h>`
- `<Wire.h>`

### ➤ Libraries Used in the Python Application:
- `serial`
- `tkinter`
- `time`
- `from tkinter: font, PhotoImage`

---

## 🖥️ How It Works

The Arduino firmware processes keypad input and performs binary arithmetic operations, displaying results on an LCD. The Python GUI communicates with the Arduino via serial protocol, enabling remote interaction and visualization of the calculator system.

---

## ⚠️ Notes

- Ensure that **Wokwi is running** before launching the Python GUI.
- The **serial communication** is set up to work with `rfc2217://localhost:4000`, so ensure it's properly configured.

---

## 👩‍💻 Author

**Sara Ghazavi**

Sharif University of Technology

Course: Computer Language and Structure – Winter 1403
