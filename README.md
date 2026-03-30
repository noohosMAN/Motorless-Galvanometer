### **Motorless PCB-Based Galvanometer (Laser Steering Module)**

**University of Windsor — ELEC-4000 Capstone Project (2025)**

---

### **Overview**

This project presents a **low-cost, motorless galvanometer system** designed for laser beam steering applications such as **Selective Laser Sintering (SLS)**, laser imaging, and optical experiments.

Traditional galvanometers rely on **precision motors and proprietary hardware**, often costing over $1000. This design replaces those components with a **PCB-based electromagnetic actuation system**, reducing total cost to **under $100** while maintaining functional 2-axis control.

The result is a **compact, reproducible, and accessible solution** for students, hobbyists, and entry-level engineering applications.

---

### **Key Features**

* Motorless **electromagnetic actuation** using PCB coils
* **2-axis mirror control** (X-Y laser steering)
* Stacked **multi-layer PCB design** for increased magnetic force
* **ESP32-based control system** with PWM signal modulation
* Lightweight **3D-printed mechanical structure**
* Fully **open-loop control with real-time visualization**
* Designed for **low-cost and reproducibility**

---

### **Performance Summary**

* Functional **2-axis laser steering demonstrated**
* Stable and repeatable mirror motion
* Real-time pattern generation (circles, Lissajous curves)
* **Total Cost:** <$100 CAD
* **Commercial Systems:** $1000–$2000+
* **Cost Reduction:** ~90%

> Note: This is a proof-of-concept system and does not yet match the precision or speed of industrial galvanometers.

---

### **System Architecture**

The system replaces traditional motors with **electromagnetic coils and permanent magnets**:

1. **PCB Coils** generate magnetic fields (multi-layer, stacked design)
2. **Neodymium magnets** mounted on a mirror platform
3. **Electromagnetic force** produces angular deflection
4. **ESP32 + motor driver** control current through coils
5. **Laser reflection** visualizes motion on a surface

---

### **Hardware Components**

* ESP32 microcontroller
* TB6612FNG dual H-bridge motor driver
* Custom 4-layer PCB coils (stacked ×3)
* Neodymium magnet array (16 magnets)
* 3D-printed mirror mount (PLA)
* Laser module

---

### **Software & Control**

* Developed using **Arduino IDE (ESP32)**
* PWM-based control for coil actuation
* Real-time signal modulation using:

  * Sinusoidal functions (sin/cos)
  * Line-drawing algorithms (Bresenham)


---

### **Design Highlights**

#### 🔹 PCB-Based Electromagnetics

* 4-layer spiral coils
* ~80 turns per PCB (240 total stacked)
* Symmetrical layout to reduce interference

#### 🔹 Mechanical System

* 3D-printed lightweight frame
* Living spring design for mirror movement
* Press-fit + modular assembly

#### 🔹 Iterative Engineering

* Initial hand-wound coil prototype → insufficient force
* Transition to stacked PCBs → successful actuation
* Migration from Arduino Nano → ESP32 for higher precision

---

### **Validation & Testing**

* Laser reflection used to track mirror motion
* Visual verification of pattern accuracy
* Iterative improvements:

  * Increased coil density
  * Added PCB stacking
  * Optimized PWM signals

---

### **Applications**

* Low-cost SLS / laser scanning systems
* Educational demonstrations (EM + control systems)
* Optical experiments
* Maker / DIY laser projects

---

### **Limitations**

* No closed-loop feedback (open-loop control only)
* Lower precision vs industrial galvanometers
* Limited force output compared to motor-driven systems

---

### **Future Improvements**

* Closed-loop feedback (position sensors)
* Higher-resolution control signals
* Improved mechanical stability
* Reduced mirror mass for faster response
* Integration into full SLS systems

