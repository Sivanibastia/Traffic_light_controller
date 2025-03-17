# Traffic_light_controller
🚦 Finite State Machine (FSM) based Traffic Light Controller for a two-street intersection, implemented in Verilog.

📌 Overview :
This project demonstrates the Traffic Light Controller using a Finite State Machine (FSM) in Verilog HDL.
The system manages traffic lights for two streets (A & B) based on vehicle presence using sensors.

🎯 Features:
✅ FSM-based Traffic Control for two streets.
✅ Vehicle Detection using sensors.
✅ Timed Light Changes (Green, Yellow, Red).
✅ Flexible Green Light Extension based on vehicle presence.
✅ Verilog Implementation & Simulation Testbench.

Traffic Light Control Logic:
Streets & Sensors:
Street A (Main Street): Default green unless a car is detected on Street B.
Street B (Side Street): Green light only when activated by a car sensor.
Timing Rules:
Street A must stay green for at least 60s.
Street B has a full cycle (red → yellow → green).
Street B’s green light extends in 10s increments if more cars are detected.
