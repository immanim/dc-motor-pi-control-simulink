PI Controller Based Motor Speed Control with Load and Friction

Overview

This project demonstrates the design and simulation of a closed-loop motor speed control system using a Proportional–Integral (PI) controller in MATLAB Simulink.

The controller regulates motor speed and compensates for external load torque and friction effects to maintain a desired reference speed.

This control strategy is widely used in electric vehicle motor drives, robotics, and industrial automation systems.

---

System Block Diagram

Reference Speed → Error Calculation → PI Controller → Motor Model → Output Speed
↑
Feedback

The controller continuously minimizes the error between the desired speed and actual motor speed.

---

PI Controller

The control signal is defined as:

u(t) = Kp·e(t) + Ki ∫ e(t) dt

Where:

- Kp = Proportional gain
- Ki = Integral gain
- e(t) = Speed error

Controller Role

Proportional control:

- Improves response speed

Integral control:

- Eliminates steady-state error

---

Simulink Model

The simulation model contains the following components:

Block| Function
Step| Reference speed input
Sum| Error calculation
Gain (Kp)| Proportional control
Integrator + Gain (Ki)| Integral control
Motor Model| Motor dynamic behavior
Load Torque| External disturbance
Friction| Mechanical damping
Scope| Displays speed response

---

Simulation Parameters

Reference Speed: 100 rad/s

Controller Gains:

Kp = 2
Ki = 1

Simulation Time: 10 seconds

---

Simulation Results

The PI controller successfully:

- Accelerates the motor quickly
- Reduces speed error
- Compensates load disturbances
- Stabilizes the system at the desired speed

---

Applications

This control strategy is used in:

- Electric Vehicle Traction Motors
- Industrial Motor Drives
- Robotics Motion Control
- Mechatronic Systems

---

Tools Used

- MATLAB
- Simulink

---

Future Improvements

Possible extensions of this project:

- Implement PID controller
- Add disturbance rejection testing
- Develop BLDC motor model
- Simulate electric vehicle traction system

---

Author

IMMANUVEL M interested in:

- Control Systems
- Electric Vehicles (EV)
- Motor Control
- Simulation and Modeling
