\# Vallorim Mk I System Requirements Specification



Version: 0.1  

Status: Draft  

Date: July 2026  



\## 1. Purpose



The purpose of Vallorim Mk I is to design, simulate, and eventually demonstrate a modular autonomous fixed-wing UAV that serves as a research platform for aerospace engineering, autonomous flight, mission planning, onboard perception, and systems integration.



The project is intended to develop both the aircraft and the supporting software ecosystem while providing a foundation for future aircraft variants and advanced autonomy research.



\## 2. Mission Objective



Vallorim Mk I is designed as a modular Intelligence, Surveillance, and Reconnaissance (ISR) research aircraft.



Primary mission objectives include:



\- Autonomous waypoint navigation

\- Long-duration stable flight

\- Modular payload integration

\- Aerial perception using onboard sensors

\- Flight dynamics and control experimentation

\- Future autonomous mission planning research



The aircraft is intended to serve as a reusable engineering platform rather than a single-purpose vehicle.



\## 3. System Overview



Vallorim Mk I consists of several major engineering subsystems:



• Airframe

• Propulsion

• Flight Computer

• Mission Computer

• Navigation System

• Sensor Suite

• Payload System

• Ground Control Station

• Simulation Environment



Each subsystem is designed to be modular, allowing future aircraft variants to reuse the same software architecture while modifying only the physical vehicle.



\## 4. Aircraft Requirements



Vallorim Mk I shall be a 1/6-scale Bayraktar TB2-inspired fixed-wing ISR/autonomy research UAV.



Baseline dimensions:



\- Wingspan: 2.00 m

\- Length: 1.08 m

\- Height: 0.37 m

\- Configuration: high-wing, twin-boom, electric pusher

\- Estimated takeoff weight: 3.0–4.5 kg

\- Payload capacity: 0.4–0.8 kg

\- Launch method: hand launch initially; rail/catapult simulation later

\- Landing method: belly landing or simple runway landing



Primary aircraft design requirements:



1\. The aircraft shall be portable enough for one person to transport.

2\. The aircraft shall support a modular payload bay.

3\. The aircraft shall prioritize stable flight over high maneuverability.

4\. The aircraft shall provide a clear forward field of view for onboard sensors.

5\. The aircraft shall be suitable for flight dynamics simulation and future autonomy development.



\## 5. Payload Requirements



Vallorim Mk I shall employ a modular payload architecture designed to support future mission expansion without requiring major airframe redesign.



\### 5.1 Baseline Payload



The baseline payload shall include:



\- Forward-facing RGB camera

\- Flight controller

\- Mission computer interface

\- GPS receiver

\- Inertial Measurement Unit (IMU)

\- Airspeed sensor

\- Barometer

\- Telemetry radio

\- Power distribution hardware



\### 5.2 Payload Bay



The aircraft shall include a modular payload bay located within the forward fuselage.



The payload bay shall:



\- Allow components to be installed or removed independently.

\- Support future payload upgrades.

\- Provide sufficient internal space for wiring and future expansion.

\- Maintain aircraft balance by locating payloads near the center of gravity whenever practical.



\### 5.3 Mission Computer



The aircraft architecture shall support an onboard mission computer.



Initially, software development may be performed on a desktop workstation. Future revisions of Vallorim Mk I shall migrate the mission computer to onboard hardware such as an NVIDIA Jetson platform without requiring significant software redesign.



\### 5.4 Future Payload Compatibility



The payload architecture shall be designed to accommodate future sensors and mission equipment, including:



\- Thermal camera

\- LiDAR

\- Multispectral camera

\- Additional onboard computing hardware

\- Experimental sensor packages



\### 5.5 Design Philosophy



The payload system shall remain independent of the airframe whenever possible.



Future aircraft variants shall be capable of reusing the same payload modules, avionics architecture, and mission computer while requiring only minimal hardware adaptation.



\## 6. Autonomy Requirements



Vallorim Mk I shall function as an autonomous research platform capable of executing pre-planned missions while allowing continuous operator supervision.



\### 6.1 Flight Autonomy



The aircraft shall support:



\- Manual flight mode

\- Stabilized flight mode

\- Autonomous waypoint navigation

\- Autonomous mission execution

\- Return-to-Launch (RTL)

\- Automatic mission termination upon critical system failures



\### 6.2 Mission Planning



The mission computer shall support:



\- Uploading waypoint-based missions

\- Modifying mission parameters prior to launch

\- Executing autonomous search patterns

\- Logging mission progress

\- Recording flight telemetry for post-flight analysis



\### 6.3 Perception



The aircraft architecture shall support onboard perception capabilities.



Future revisions shall support:



\- Object detection

\- Object tracking

\- Terrain awareness

\- Landing zone identification

\- Visual target localization



The perception system shall be modular so that algorithms may be upgraded independently of the aircraft.



\### 6.4 Navigation



The aircraft shall utilize multiple navigation sensors including:



\- GPS

\- IMU

\- Barometer

\- Airspeed sensor



The software architecture shall support future sensor fusion improvements.



\### 6.5 Safety



The autonomous system shall prioritize safe operation.



Minimum safety functions shall include:



\- Return-to-Launch upon communication loss

\- Low battery failsafe

\- Flight termination upon critical hardware failure

\- Manual pilot override at any time



\### 6.6 Future Capabilities



The Vallorim software architecture shall be designed to support future autonomy research including:



\- AI-assisted mission planning

\- Multi-aircraft coordination

\- Collaborative autonomy

\- Vision-based navigation

\- GPS-denied navigation

\- Autonomous payload management



These capabilities are not required for Vallorim Mk I but shall be considered during software architecture design.



\## 7. Simulation Requirements



Vallorim Mk I shall be developed using a simulation-first engineering approach.



Simulation shall be used to verify aircraft performance, flight software, autonomy algorithms, and mission planning before hardware integration.



\### 7.1 Flight Dynamics



The simulation environment shall support:



\- Fixed-wing aircraft dynamics

\- Aerodynamic performance analysis

\- Control surface modeling

\- Propulsion modeling

\- Aircraft stability analysis



\### 7.2 Software-in-the-Loop (SITL)



The software architecture shall support Software-in-the-Loop (SITL) testing.



The simulation environment shall allow validation of:



\- Flight controller behavior

\- Autonomous waypoint missions

\- Return-to-Launch functionality

\- Mission execution

\- Flight safety logic



without requiring a physical aircraft.



\### 7.3 Sensor Simulation



The simulation environment shall support simulated sensor inputs including:



\- GPS

\- IMU

\- Barometer

\- Airspeed sensor

\- Camera imagery



Future revisions may include simulated LiDAR, thermal cameras, and additional payload sensors.



\### 7.4 Mission Simulation



The aircraft shall be capable of executing complete autonomous missions in simulation.



Simulation shall support:



\- Waypoint navigation

\- Search patterns

\- Emergency procedures

\- Mission interruption

\- Return-to-Launch



\### 7.5 Computer Vision Simulation



The simulation environment shall support development and testing of onboard perception algorithms.



Initial objectives include:



\- Object detection

\- Object tracking

\- Image processing

\- Camera data recording



Future revisions may support terrain awareness and visual navigation.



\### 7.6 Verification Philosophy



Whenever practical, new software shall be validated in simulation before being deployed to physical hardware.



Simulation shall serve as the primary development environment throughout Vallorim Mk I.



\## 8. Software Requirements



The Vallorim software architecture shall be modular, scalable, and reusable across future aircraft variants.



Software components shall be designed to operate independently while communicating through well-defined interfaces.



\### 8.1 Flight Control Software



The flight control system shall provide:



\- Aircraft stabilization

\- Flight mode management

\- Navigation command execution

\- Flight safety monitoring

\- Sensor integration



The flight controller shall remain independent from high-level autonomy software.



\---



\### 8.2 Mission Computer



The mission computer shall provide:



\- Mission planning

\- Autonomous decision making

\- Payload management

\- Sensor processing

\- Communication with the flight controller



The mission computer architecture shall support future onboard computing platforms without requiring significant software redesign.



\---



\### 8.3 Ground Control Station



The ground control station shall provide:



\- Mission upload

\- Telemetry monitoring

\- Flight visualization

\- System health monitoring

\- Flight log retrieval

\- Manual operator override



The ground station shall supervise the aircraft but shall not be required for autonomous mission execution.



\---



\### 8.4 Computer Vision



The software architecture shall support future onboard perception capabilities including:



\- Object detection

\- Object tracking

\- Image classification

\- Image recording

\- Future visual navigation research



Perception software shall remain modular and independently upgradeable.



\---



\### 8.5 Data Logging



The aircraft shall record operational data including:



\- GPS position

\- Aircraft attitude

\- Airspeed

\- Altitude

\- Battery status

\- Flight mode

\- Mission events



Recorded data shall be available for post-flight analysis.



\---



\### 8.6 Communications



The software architecture shall support communication between:



\- Flight controller

\- Mission computer

\- Ground control station



Communication interfaces shall be modular to support future hardware upgrades.



\---



\### 8.7 Software Design Philosophy



Software developed for Vallorim shall emphasize:



\- Modularity

\- Reliability

\- Reusability

\- Maintainability

\- Scalability



Whenever practical, new software shall be validated in simulation prior to hardware deployment.

\## 9. Constraints



The design and development of Vallorim Mk I shall be subject to the following constraints.



\### 9.1 Project Timeline



The Vallorim Mk I project shall be designed for completion within approximately one year while the primary developer completes an undergraduate degree.



\### 9.2 Budget



The project shall prioritize commercially available components and open-source software whenever practical.



Major hardware purchases shall occur only after software and simulation have demonstrated sufficient maturity.



\### 9.3 Portability



The aircraft shall be transportable by one person and capable of being stored within a standard passenger vehicle.



\### 9.4 Modularity



Major aircraft subsystems shall be replaceable or upgradeable without requiring complete redesign of the aircraft.



These subsystems include:



\- Payload system

\- Mission computer

\- Flight controller

\- Sensor suite

\- Power system



\### 9.5 Safety



The project shall prioritize safe engineering practices throughout development.



Simulation shall be used as the primary validation environment before hardware integration.



Physical testing shall only be conducted after sufficient verification has been completed.



\### 9.6 Scalability



Engineering decisions made during Vallorim Mk I shall support future aircraft variants including larger aircraft, VTOL aircraft, and expanded autonomous capabilities.



\### 9.7 Documentation



Major engineering decisions shall be documented throughout the project.



Design reviews, requirements updates, software architecture, CAD revisions, and testing results shall be maintained within the Vallorim repository.



\### 9.8 Open Architecture



The system architecture shall remain sufficiently modular to allow future integration of new hardware, software, and payload technologies with minimal redesign.



\## 10. Success Criteria



Vallorim Mk I shall be considered successfully completed when the following engineering objectives have been achieved.



\### 10.1 Aircraft Design



\- A complete CAD model of the aircraft has been developed.

\- Aircraft geometry, structure, and major subsystems have been documented.

\- The airframe supports a modular payload architecture.



\---



\### 10.2 Simulation



\- The aircraft has been modeled in a flight simulation environment.

\- Flight characteristics have been validated through simulation.

\- Autonomous missions have been successfully demonstrated in simulation.



\---



\### 10.3 Flight Software



The software architecture successfully supports:



\- Flight control

\- Mission planning

\- Ground station communication

\- Telemetry logging

\- Autonomous waypoint navigation



\---



\### 10.4 Perception



The aircraft demonstrates onboard perception capabilities including:



\- Object detection

\- Object tracking

\- Image recording



The perception software shall operate using an onboard mission computer or an equivalent development environment.



\---



\### 10.5 Documentation



The Vallorim repository shall contain:



\- System Requirements Specification

\- Design Decisions

\- Software Architecture

\- CAD Documentation

\- Engineering Drawings

\- Design Reviews

\- Testing Reports

\- Flight Logs

\- Project Roadmap



\---



\### 10.6 Engineering Process



The project shall demonstrate the complete engineering lifecycle including:



\- Requirements definition

\- Concept development

\- Trade studies

\- CAD design

\- Simulation

\- Software development

\- System integration

\- Verification and validation

\- Final documentation



\---



\### 10.7 Future Expansion



The final architecture shall support future development of Vallorim Mk II without requiring major redesign of the software architecture.



Future expansion may include:



\- VTOL/STOL capability

\- Advanced onboard AI

\- Additional payload systems

\- Collaborative multi-aircraft operations

\- Expanded autonomous mission capabilities

