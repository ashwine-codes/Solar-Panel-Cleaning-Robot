# Solar-Panel-Cleaning-Robot
A lightweight, brush-based robotic system to clean solar panels using a dry or wet mechanism, controlled via ESP32 and cloud-monitored through ThingSpeak. Designed to maintain up to 90% panel efficiency, even in dusty environments.

# Components Used 
* Hardware:
1. ESP32 Microcontroller
2. L298N Motor Driver
3. DC Geared Motors
4. Brush System
5. IR Sensors (IR1, IR2)
6. LDRs (Light Dependent Resistors)
7. Water Sprinkler + Pump
8. Power Supply + Battery

* Software:
1. Arduino IDE
2. ThingSpeak IoT Dashboard

# Working Overview
- The robot starts from a parking station and moves across solar panels.
- IR sensors detect panel edges to guide motion.
- LDRs provide sunlight tracking input.
- Cleaning is performed via dry brush or water-sprayed brush.
- ThingSpeak logs motor run status and temperature/humidity via DHT11.

# Functional Flow
1. Standby Mode: Charges at parking station.
2. Activation: Triggered manually or via cloud.
3. Brush Action: Motorized brush cleans the panel surface.
4. Sun Tracking: LDRs detect optimal angle for cleaning.
5. Auto Return: Robot resets to the base when cleaning completes.

# Results
- 50% drop in current when dusty; restored up to 90% after cleaning.
- Efficient energy recovery post-cleaning.
- Scalable solution for large solar farms.

# Documentation: 
Research paper: https://www.tijer.org/tijer/papers/TIJER2305338.pdf
