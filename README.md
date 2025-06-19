# PIKAPCB


---

### **What This Circuit Does**  
1. **Single-Button Control** (Keychain Switch):  
   - Press the button to **turn on 2 LEDs and the vibrating motor simultaneously**.  
   - Release to turn everything off.  

2. **Automatic Light Sensor (Optional LDR Mode)**:  
   - If you included an LDR, the LEDs can also turn on **automatically in darkness**.  

3. **Compact Design**:  
   - Powered by a **small battery (e.g., coin cell or 3V CR2032)** for portability.  

---

### **Design Choices & Challenges**  
#### **Why This Design?**  
- **Keychain Use Case**: You wanted a simple, one-handed operation (no need for two-button safety).  
- **Minimalist Parts**: Reduced components to fit a small enclosure (e.g., keychain or pocket-sized).  

#### **Challenges Faced**  
- **Power Management**: Ensuring the battery can drive both LEDs and motor without draining too fast.  
   - *Fix*: Use low-current LEDs (e.g., 2mA) and a efficient motor (3V pager motor).  
- **Space Constraints**: Fitting everything into a tiny keychain form.  
   - *Fix*: SMD components or tightly arranged through-hole parts.  

#### **What I Learned**  
- **KiCad Tips**:  
  - Use **global labels** (e.g., `+VCC`, `GND`) to avoid messy wires.  
  - **ERC Checks** catch missing power connections early.  
- **Circuit Simplification**: Fewer parts = fewer points of failure.  

---

### **Advice for Beginners**  
1. **Start Simple**:  
   - If this is your **first PCB**, try a **single-LED + button circuit** before adding motors/sensors.  
2. **KiCad Learning Curve**:  
   - Watch tutorials on **schematic symbols** vs. **footprints** (common confusion).  
3. **Test on Breadboard First**:  
   - Verify the circuit works before designing the PCB.  

---

### **Optional Upgrades**  
1. **Add a Timer (555 IC)**:  
   - Make the motor vibrate for **10 seconds after button press**.  
2. **Low-Power Mode**:  
   - Use a **toggle switch** to disable the motor but keep LEDs.  

---

