# Description 
Cor is an wearable electronic device that monitors your heart rate and using real data could use heart rates over periods of time to detect diseases which you could check with your doctor
# Purpose 
The purpose of Cor is for people with diseased hearts to be moitner the condtion of their heart and relay the information to a Doctor
# Items
---
### 1. Core Processing & Silicon
*   **Raspberry Pi Pico H Microcontroller Board**
    *   *Specification:* RP2040 chip, dual-core ARM Cortex-M0+, 2MB flash memory, pre-soldered 0.1-inch pitch male pin headers.
    *   *Purpose:* Central processing unit for running the diagnostic system loop, managing the shared SPI bus, and refreshing the interface.
    *   *Estimated Price:* \$7.50 CAD
*   **MAX30102 Pulse Oximeter & Heart Rate Sensor Module**
    *   *Specification:* Integrated optical biosensor, dual LEDs (660nm Red and 880nm Infrared) with ambient light cancellation circuitry, low-noise analog front-end.
    *   *Purpose:* Reads raw photoplethysmography (PPG) volume signals through the skin layer on the wrist via the I2C bus.
    *   *Estimated Price:* \$11.00 CAD
*   **2.4-inch TFT LCD Display Module with Touch Panel**
    *   *Specification:* 240x320 pixels resolution, 65K color depth, SPI communication interface, driven by the ILI9341 display controller chip paired with the XPT2046 resistive touch panel digitizer chip.
    *   *Purpose:* Shows live heart waveforms, health metrics, textual system alerts, and accepts tactile user navigation controls.
    *   *Estimated Price:* \$18.00 CAD

---

### 2. Power Delivery & Management
*   **3.7V 500mAh Lithium-Polymer (LiPo) Rechargeable Battery**
    *   *Specification:* Flat prismatic form factor (Model 503035), nominal 3.7V voltage, integrated over-discharge/short-circuit protection PCM circuit board.
    *   *Purpose:* Provides portable, thin-profile power directly tucked into the central sandwich cavity of the watch housing.
    *   *Estimated Price:* \$9.50 CAD
*   **TP4056 Lithium Battery Charger & Safety Module**
    *   *Specification:* Constant-Current/Constant-Voltage (CC/CV) linear charging management chip, USB Type-C or Micro-USB input terminal, dual onboard status LEDs.
    *   *Purpose:* Standardized recharging port that regulates current down to prevent overcharging or swelling the compact internal battery pack.
    *   *Estimated Price:* \$2.50 CAD
*   **Miniature SPDT Slide Switch**
    *   *Specification:* Single-Pole Double-Throw, through-hole right-angle sub-miniature toggle action rated for 0.3A at 5V DC.
    *   *Purpose:* Hardware on/off power switch breaks or connects the main positive battery line to isolate power safely when the device is not worn.
    *   *Estimated Price:* \$1.50 CAD

---

### 3. Physical Interconnects & Structural Elements
*   **22mm Adjustable Nylon Loop Watch Strap**
    *   *Specification:* Heavy-duty woven ballistic nylon weave, infinite adjustment via integrated micro-hook-and-loop velcro closures, lightweight breathable fiber structure.
    *   *Purpose:* Attaches the watch case to the wrist and keeps constant, uniform skin pressure against the bottom optical module window.
    *   *Estimated Price:* \$8.00 CAD
*   **Custom 3D-Printed Watch Chassis & Internal Mount Brackets**
    *   *Specification:* ~45 grams of high-impact PLA or PETG thermoplastic filament material output at 0.16mm layer height resolution.
    *   *Purpose:* Mechanical enclosure shell providing precise standoffs for internal boards, a structural watch bezel, and an ambient light-blocking lens shield ring.
    *   *Estimated Price:* \$2.00 CAD (pro-rated material cost)
*   **Mechanical Sockets & Connecting Wire Bundles**
    *   *Specification:* High-flexibility 28 AWG silicone-insulated multi-strand hookup wire lines, ultra-low profile M2 self-tapping engineering screws (4mm length).
    *   *Purpose:* Internal electrical connections between components and structural fastening of board plates into case bosses.
    *   *Estimated Price:* \$3.00 CAD

---

### 4. Embedded Firmware Drivers & Software Assets
*   **MicroPython Core Firmware Runtime Environment**
    *   *Version:* Official Raspberry Pi Pico firmware binary drop (`.uf2`).
    *   *Purpose:* Lightweight interpretive language engine operating directly on top of the silicon layer.
    *   *Estimated Price:* \$0.00 (Open-Source Free Asset)
*   **`micropython-max30102` Control Module Driver**
    *   *Purpose:* Handles specific I2C configurations, register read cycles, configuration parameters, and manages the internal FIFO data pipeline of the optical sensor.
    *   *Estimated Price:* \$0.00 (Open-Source Free Asset)
*   **`ili9341` Hardware Accelerated Screen SPI Driver**
    *   *Purpose:* Graphic frame drawing commands, text layouts, geometric renderings, and hardware coordinate optimization scripts.
    *   *Estimated Price:* \$0.00 (Open-Source Free Asset)
*   **`xpt2046` Intercept Coordinate Matrix Touch Driver**
    *   *Purpose:* Maps continuous interrupt pin polling data and maps physical coordinate positions into software click events.
    *   *Estimated Price:* \$0.00 (Open-Source Free Asset)
