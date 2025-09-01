# Project-Overview

![Decorative blueprint of airplane design](/assets/blueprint_background.png)

The Advanced UAV Research Association is a project based club focused on designing, building, and testing a high speed autonomous airplane. The project emphasizes hands-on engineering, collaboration, and applied research in software, hardware, and avionics. This roadmap is iterative and tentative as we learn and research new technologies.


## Project Goals
- 100+ mph
- Autonomous flight
	- Ability to follow gps waypoint missions
	- Auto take off and landing
- Develop and build flight computer from scratch
	- Design flight computer board
	- Design flight software
- Develop and build airframe


## Roadmap
The following is a rough roadmap of the project, subject to change.
The goal is to complete the key project goals outlined earlier by the end spring 2026.

| Phase | Goal | Hardware Development | Software Development | Key Milestones |
|-------|------|----------------------|----------------------|---------------|
| **Phase 1<br/>MVP Development** | Establish basic flight capability with minimal viable product | • Use pre-built aircraft platform<br>• Raspberry Pi mounted to perf board<br>• Basic sensor suite | • Rapid Python development for initial flight control<br>• Basic HAL implementation in C++<br>• Synthetic data testing environment<br>• Basic PID control with rudimentary filtering | • Manual flight capability<br>• Basic autonomous functions (straight line, simple turns)<br>• HAL-flight software integration |
| **Phase 2<br/>Autonomous Foundation** | Create basic autonomous system with validation framework | • Premade slow-speed airframe<br>• Expanded sensor integration<br>• Begin 3D printing exploration for custom parts | • Test-driven development approach<br>• Validation/simulation suite development<br>• Refined HAL layer with additional sensors<br>• Architecture stabilization | • Waypoint following capability<br>• Comprehensive automated testing framework<br>• Flight dynamics categorization<br>• Initial self-design research |
| **Phase 3<br/>Flight Dynamics Validation** | Develop algorithms for high-speed characteristics | • Custom airframe approximating high-speed dynamics<br>• Optimized hardware configuration | • High-performance C++ implementation<br>• Real-time OS optimizations<br>• Advanced control algorithms (MPC)<br>• Automated takeoff/landing systems | • Validated control algorithms<br>• SIL (Software-in-Loop) testing suite<br>• Stable autonomous flight at intermediate speeds |
| **Phase 4<br/>High-Speed Implementation** | Achieve 100+ mph autonomous flight | • Custom-designed high-speed airframe<br>• Optimized EDF propulsion system<br>• Final flight computer hardware | • Robust real-time Linux implementation<br>• Feature-freeze on core control loops<br>• Comprehensive verification & testing | • Consistent 100+ mph autonomous flight<br>• Reliable automated takeoff/landing<br>• Mission-ready system for potential applications |

*Possible Future Development: Higher speed capabilities, advanced navigation systems, environmental awareness, and mapping functionality.*

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
