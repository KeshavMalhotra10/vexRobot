# Hospital Navigation & Delivery Robot - vexRobot

Mechatronics Systems Project
👥 Team Members

Keshav Malhotra
Rohan Raina
Caden Brown
Tucker Johnson

🩺 Project Overview
Hospitals are often difficult to navigate, especially for patients and visitors unfamiliar with their complex layouts. At the same time, the ongoing nursing shortage has left medical staff with heavy workloads, slowing the delivery of critical medications.
Inspired by real-world hospital experiences, our project aims to solve both issues through a single autonomous solution: a hospital navigation and delivery robot.
This robot will serve two primary roles:

Autonomous Guide – Helping patients and visitors move through hospital corridors.
Delivery Assistant – Transporting medical supplies between departments.

By combining navigation, delivery, and automation, the system reduces staff workload and ensures smoother hospital operations.
⚙️ Key Features
Motion & Control

Dual motors to drive and steer the robot.
One motor dedicated to opening and closing a medical storage box.

Sensors & Inputs

Remote Control for route training.
Encoders for distance tracking.
Touch Sensor for box activation.
Bumper Sensor for collision detection.
Optical Sensor to identify drop-off zones.
Gyro Sensor to maintain straight movement and accurate turns.
Distance Sensor to slow the robot as it nears obstacles.

Automation Logic

Timer ensures the robot returns to base if the box isn't opened in time.
Continuous feedback loops for movement correction.
Distinct training and autonomous operation modes.

🧠 Core Functions

recordPath() – Records user-driven routes for autonomous playback.
reversePath(path) – Reverses a stored route for return trips.
executePath(path) – Executes stored routes automatically.
controlBox(isOpen) – Opens or closes the storage box.
drive(distance, direction) – Controls forward/backward movement.
turn(angle) – Rotates robot to a specific orientation.
calculateSpeed(distance) – Adjusts speed based on proximity to obstacles.
