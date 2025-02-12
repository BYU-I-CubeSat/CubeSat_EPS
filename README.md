# CubeSat_EPS
Electrical Power System (EPS) manages the power collection and distribution in the satellite with an integrated Battery Management System (BMS).

# CubeSat EPS Component List

This document provides a comprehensive list of all components required to design and build a low-cost Electrical Power System (EPS) for a 1U CubeSat operating in Low Earth Orbit (LEO).

## **1. Power Generation (Solar Panels & Energy Harvesting)**
- **Solar Cells** (Triple-junction GaAs or Silicon)
- **Bypass Diodes** (Schottky diodes for panel protection)
- **Interconnects** (Flexible PCB or wire bonding for panel connections)
- **Encapsulation Material** (Covers for protection against radiation & debris)
- **Deployable Panel Hinges** (If using deployable solar arrays)
- **Deployment Mechanism** (Springs, burn wire, or SMA actuators)

## **2. Power Storage (Battery Subsystem)**
- **Lithium-Ion or LiFePO4 Battery Cells** (Typically 18650 or pouch cells)
- **Battery Management System (BMS) IC**
  - Overcharge protection
  - Over-discharge protection
  - Cell balancing
  - Temperature monitoring
- **Thermistors/Temperature Sensors** (For thermal management)
- **Battery Holders or Enclosure**
- **Fuses** (For additional battery protection)

## **3. Power Regulation & Distribution**
- **Maximum Power Point Tracking (MPPT) Controller IC**
- **DC-DC Converters**
  - **Buck Converters** (Step-down voltage regulation, e.g., 5V, 3.3V, 12V rails)
  - **Boost Converters** (Step-up voltage regulation if needed)
- **Low Dropout Regulators (LDOs)** (For noise-sensitive circuits)
- **MOSFETs & Switching Components** (For power routing & load switching)
- **Current Sense Resistors** (For power monitoring & safety)
- **Inductors & Capacitors** (For DC-DC converter stability)
- **Protection Diodes** (Prevent reverse voltage damage)

## **4. Power Monitoring & Telemetry**
- **Microcontroller/Processor** (Handles power telemetry & control)
- **ADC (Analog-to-Digital Converter)** (Reads voltage & current sensor data)
- **I2C or SPI Communication Interface** (For data transmission to OBC)
- **Shunt Resistors** (For current measurement)
- **Operational Amplifiers (Op-Amps)** (Signal conditioning for ADC readings)
- **Temperature Sensors** (Battery and PCB thermal monitoring)
- **EEPROM/FRAM** (For storing telemetry data if needed)

## **5. Power Safety & Fault Protection**
- **Polyfuses/Resettable Fuses** (Overcurrent protection)
- **TVS Diodes** (Transient voltage suppression against surges)
- **Schottky Diodes** (Prevent reverse polarity damage)
- **Isolation Relays or Solid-State Switches** (For controlled power distribution)
- **Watchdog Timer IC** (Resets EPS in case of lock-up)

## **6. Connectors & Wiring**
- **Board-to-Board Connectors** (For modular design and integration with OBC & payload)
- **PCB Terminals** (For secure wire connections)
- **Power Distribution Board (PDB) PCB** (For routing power safely)
- **Harnessing (Wires & Flex Cables)**
- **Connectors (Molex, JST, or Samtec)**
- **Screw Terminals or Solder Pads** (For battery connection and power lines)

## **7. Structural & Thermal Considerations**
- **PCB Mounting Hardware** (Standoffs, screws, thermal pads)
- **Thermal Interface Materials (TIMs)** (Improve heat dissipation)
- **Heatsinks (If necessary)** (For hot components like power regulators)
- **Kapton Tape & Insulation** (Electrical insulation & protection)
- **Conformal Coating** (For protection against radiation and moisture)

## **8. Software & Firmware Considerations**
- **Power Management Firmware** (Controls MPPT, battery charging, and telemetry)
- **Fault Handling & Recovery Code** (Self-reset and protection mechanisms)
- **Communication Protocols** (I2C, SPI, UART for data exchange with OBC)
- **Telemetry Data Logging** (Stores EPS performance for analysis)

## **Optional Components (Mission Dependent)**
- **Redundant Power Paths** (For improved reliability)
- **Supercapacitors** (For power buffering during peak loads)
- **Wireless Power Transfer Modules** (If required for special applications)
- **Electromagnetic Interference (EMI) Shielding** (For noise-sensitive components)

### **Conclusion**
This list covers every essential component needed for a robust and cost-effective CubeSat EPS. Team members should review and refine the selection based on the specific mission requirements, budget constraints, and testing needs.

