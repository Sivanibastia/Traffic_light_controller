# Traffic_light_controller
Traffic Light Controller Using Finite State Machine (FSM)
This project implements a traffic light controller using a finite state machine (FSM) to manage traffic at an intersection with two streets: Street A (main street) and Street B.

Specifications:
Street A: Defaults to green if no cars are detected; must remain green for at least 60 seconds.
Street B: Green light for a minimum of 50 seconds; can extend green in 10-second increments if cars are detected.
Implementation:
The FSM operates on a clock with 10-second increments.
States include:
Reset (Street A green, Street B red)
Yellow for Street A
Green for Street B
Transitions are based on sensor inputs from each street.

