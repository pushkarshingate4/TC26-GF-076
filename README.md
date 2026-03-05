# TC26-GF-076

# Cubix Logic 

### Modular Magnetic Embedded Learning Platform

Cubix Logic is a **modular embedded learning platform** designed to help students understand **electronics, sensors, digital logic, and embedded systems** through a hands-on cube-based architecture.

Each cube represents a **separate electronic module** such as sensors, logic gates, processors, or output devices. Learners can physically assemble these cubes to build working electronic systems while understanding the **Input → Processing → Output (IPO)** model. 

---

# System Overview

Cubix Logic uses **magnetically connected cubes** to create a safe, wire-free learning environment.

Each cube acts as a subsystem:

* **Input Modules** – Sensors (Ultrasonic, Touch, LDR)
* **Processing Module** – ESP32 Controller
* **Logic Modules** – AND, OR, XOR Gate Cubes
* **Output Modules** – LED, Display, Buzzer

Students assemble cubes to create complete embedded systems while observing real-time responses.

---

# Core Concept: Controlled Modular Dependency

Cubix Logic follows a strict **Input → Processing → Output architecture**.

<img width="885" height="377" alt="image" src="https://github.com/user-attachments/assets/8268c46a-cde1-4863-82c9-ffa84a6089b6" />


A key rule in the system:

 **Sensor cubes remain inactive unless a compatible output cube is connected.**

This rule is enforced using:

* Hardware power routing
* Firmware validation through ESP32

This ensures learners understand **real embedded system dependencies**, instead of random component connections. 

---

#  Magnetic Conductive Cube System

The platform uses **Neodymium magnets and copper contact pads** to connect cubes.

<img width="867" height="432" alt="image" src="https://github.com/user-attachments/assets/1d949cef-8d58-4c99-9c31-4ef5a04e28ec" />


### Functions of the Magnetic Interface

* Mechanical alignment
* Electrical power transfer
* Signal communication
* Correct orientation validation

### Key Design Features

**Magnetic Alignment**

* Cubes automatically align using fixed-polarity magnets.

**Orientation Control**

* Incorrect rotation causes magnetic repulsion or misalignment.

**Copper Electrical Contacts**

* Copper pads handle power and signal transmission.
* Magnets only provide alignment.

**Stable Power Distribution**

* Power is delivered only when pads are fully aligned.
* Partial contact prevents system activation.

This design removes the need for **wires or connectors**, making the system safer and easier to use in classrooms. 

---

#  Base Platform and Controller

The **ESP32 controller base** acts as the central hub.

### Responsibilities

* Power distribution
* Detecting cube placement
* Validating module combinations
* Processing sensor data
* Activating output devices

### System Logic

| Condition              | System Behavior          |
| ---------------------- | ------------------------ |
| No output cube         | Sensors remain disabled  |
| Invalid cube placement | System stays inactive    |
| Valid sensor + output  | System operates normally |

This models **real embedded system configuration behavior**.

---

#  Sensor Cubes (Input Modules)

Sensor cubes collect environmental data and send it to the ESP32.

## Ultrasonic Sensor Cube

* Measures distance using ultrasonic waves
* Demonstrates **time-of-flight sensing**

## Touch Sensor Cube

* Detects capacitive touch
* Demonstrates **event-based inputs**

## LDR Sensor Cube

* Measures light intensity
* Uses ESP32 **ADC conversion**

Sensors only activate when **an output cube is connected**.

---

#  Logic Gate Cubes

Logic gate cubes work **independently from the ESP32** and demonstrate digital logic concepts.

| Cube     | Function                             |
| -------- | ------------------------------------ |
| AND Gate | Output HIGH when all inputs are HIGH |
| OR Gate  | Output HIGH when any input is HIGH   |
| XOR Gate | Output HIGH when inputs differ       |

These cubes help students understand **Boolean logic in hardware form**.

---

#  Output Cubes

Output cubes provide system feedback.

### LED Cube

Binary visual indication.

### Display Cube

Shows numerical sensor values.

### Buzzer / Speaker Cube

Provides audio alerts.

Output cubes also **activate sensor modules**, completing the IPO system.

---

#  Safety Features

* Low-voltage operation
* Enclosed electronics
* No exposed wiring
* Magnetic alignment prevents wrong connections
* Firmware checks ensure valid system configuration

---

#  Educational Impact

Cubix Logic converts abstract electronics concepts into **interactive physical learning**.

Students learn:

* Embedded system architecture
* Sensor interfacing
* Digital logic
* Hardware validation
* System dependencies

The modular magnetic design makes it ideal for **STEM education, robotics labs, and innovation competitions**.

---

# 🚀 Conclusion

Cubix Logic is a **modular magnetic embedded learning platform** that allows learners to physically build and understand real embedded systems. By combining **magnetic alignment, controlled electrical connections, and ESP32 processing**, the system ensures safe, reliable, and meaningful hands-on learning.

---
