# Arduino Binary Calculator with Python GUI

This project consists of an **Arduino-based binary calculator simulation** and a **Python GUI application**. The calculator is designed to run on the Wokwi simulator, and the Python application provides a graphical interface for interacting with it.

## 📂 Project Structure

```
BINARYCALCULATOR/
│── .vscode/
│── sketch/
│   ├── sketch.ino      # Arduino simulation code
│── app.py              # Python GUI application
│── calculator.png      # Icon for the application
│── diagram.json        # Wiring diagram
│── libraries.txt       # Required libraries
│── README.md           # Documentation
│── sketch.ino.elf      # Compiled ELF file
│── sketch.ino.hex      # Compiled HEX file
│── wokwi-project.txt   # Wokwi project details
│── wokwi.toml          # Wokwi configuration
```

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
