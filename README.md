# Traffic_light_controller
Overview of Traffic Light Controller Using Finite State Machine (FSM)

The video demonstrates the use of a finite state machine (FSM) to control a traffic light system.

The system involves two streets: Street A (main street) and Street B.

Each street is equipped with sensors to detect vehicle presence.

Traffic Light Control Specifications

Street A is the main street and defaults to green if no cars are detected.

When activated, Street A must remain green for at least 60 seconds.

Street B's light sequence includes red, yellow, and green, with a minimum green duration of 50 seconds.

If cars are detected on Street B while Street A is clear, the green light for Street B can be extended in 10-second increments.

The FSM will manage the light changes based on sensor inputs and timing.

Implementation Details

The FSM operates on a clock with a 10-second increment for simplicity.
The design includes various states for traffic light control, with each state lasting 10 seconds.
The states include:
Reset state for Street A (green) and Street B (red).

Intermediary state for preparing to stop (yellow for Street A).

Green for Street B and red for Street A.

Transition states based on sensor inputs.

FSM Design and Coding

The FSM requires 13 states, necessitating a 4-bit representation.

The code includes sequential state logic and next state logic.

The transitions between states are primarily based on sensor inputs.

Outputs are defined for each state to control the traffic lights (red, yellow, green).

Test Bench and Simulation

A test bench is created to validate the FSM implementation.
The test bench simulates various scenarios, including:
Initial state with no cars detected.
Activation of Street B when no cars are on Street A.
Transitioning to Street A when a car is detected.
The simulation results confirm the expected behavior of the traffic light controller, with clear outputs for each light state.
