# LPC2148 ADC LCD Display

This project reads analog values from two potentiometers using the LPC2148 ARM7 microcontroller’s built-in ADC channels and displays them on a 16x2 LCD in 4-bit mode.

---

## 🧠 Features

- Reads analog voltage on **ADC Channel 2 and 3**
- Converts analog input to 10-bit digital values
- Displays the values on **16x2 LCD**
- Uses **PLL initialization** for stable clocking
- Modular code using:
  - `PLL.h`
  - `Lcd_4bit.h`
  - `ADC.h`

---

## 📷 Hardware Used

- NXP **LPC2148** ARM7 Microcontroller
- 2 × Potentiometers (connected to P0.28 and P0.29)
- 16x2 LCD (in 4-bit mode)
- Power supply (3.3V/5V regulated)
- Crystal oscillator (12 MHz)

---

## 🔌 Pin Connections

| LCD Pin | LPC2148 Pin |
|---------|--------------|
| RS      | P0.10        |
| EN      | P0.11        |
| D4-D7   | P0.12-P0.15  |

| ADC Channel | Pin        | Description       |
|-------------|------------|-------------------|
| ADC2        | P0.28      | Potentiometer 1   |
| ADC3        | P0.29      | Potentiometer 2   |

---

## 🛠️ How to Run

1. Open the project in **Keil uVision** or other supported IDE.
2. Compile and flash the code using **Flash Magic** or UART programmer.
3. Power the board and turn the potentiometers.
4. See real-time ADC values on the LCD.

---

## 📁 File Structure

LPC2148_ADC_LCD_Display/
├── ADC.h # ADC initialization and read function
├── PLL.h # Clock setup using Phase Locked Loop
├── Lcd_4bit.h # LCD control functions
├── main.c # Main logic (read ADC and display)
├── Two_ADC_pote.uvproj # Keil project file
└── README.md # Project description


---

## 📜 License

This project is open-source and free to use for academic or personal purposes.

---

## ✍️ Author

**Sanket Mali**  
[GitHub](https://github.com/Sanketmail3716)

