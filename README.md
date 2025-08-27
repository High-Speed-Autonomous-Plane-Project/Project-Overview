# Project-Overview
The Advanced UAC REsearch Organization is a project based club focused on designing, building, and testing a high speed autonomous airplane. The project emphasizes hands-on engineering, collaboration, and applied research in software, hardware, and avionics. This roadmap is iterative and tentative as we learn and research new technologies.

| Phase                                | Focus                  | Key Goals                                                                                                                                                       |
| ------------------------------------ | ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Phase 1:** Proof of Concept        | Manual RC Plane        | Foam-board design, manually controlled RC plane, basic flight stability testing (\~fast-ish speeds).                                                            |
| **Phase 2:** Structured Development  | Organized Architecture | Introduce modular hardware/software, Python-based high-level controls, reusable **Hardware Abstraction Layer (HAL)**, manual takeoff, target speed 100–200 mph. |
| **Phase 3:** Optimization & Autonomy | Advanced Control       | Migrate to optimized C/C++ software, custom PCB design, autonomous navigation and takeoff, refine control algorithms, target speed 200 mph.                     |
| **Phase 4:** Fully Autonomous UAV    | Feature Expansion      | High-speed, fully autonomous aircraft with advanced features (mapping, sensor integration).                                                                     |

## Software 
Software focuses on developing the flight computer and control systems:
* Platform: Embedded Linux on Raspberry Pi 02W
* Firmware:
    * Written in C/C++ (ELF executables)
    * Flight controller logic, servo/motor control
    * Sensor integration: IMU, GPS, Battery Management System (BMS), RC receiver
* Drivers:
  * Flight controller driver
  * GPS and sensor drivers
  * Motor/servo control drivers
* Flight Computer Architecture:
  * Realtime
    * Real-time control loops, filtering algorithms
    * Control algorithms for stability
  * Delayed
    * Navigation algorithms (Bezier curves, heuristic A* pathfinding)
    * Logging and telemetry

## Hardware
Hardware development ensures robust, modular, and scalable avionics:
* Hardware Abstraction Layer (HAL): Converts raw sensor data to meaningful SI units (when applicable)
* PCB Design:
  * Custom board integrating Pi02W, IMU, GPS, servos, motor controllers
* Control Systems:
  * Manual RC backup control
  * Planned LiDAR integration for obstacle detection

## Research
Research underpins all development by:
* Evaluating existing UAV frameworks and code libraries
* Investigating advanced navigation, sensor fusion, and flight dynamics
* Identifying off-the-shelf components for cost-effective prototyping
* Documenting findings for member onboarding and future iterations

Overview documents, timelines, roadmaps, etc.
