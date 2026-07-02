\# Vallorim Design Decisions



\---



\# Decision 001 – Program Purpose



Vallorim exists to develop a modular, multirole autonomous aircraft platform and the software ecosystem behind it. The project serves as a long-term aerospace engineering research platform for aircraft design, autonomous flight, onboard perception, mission planning, and future defense-oriented autonomy research.



Reason:

Rather than building a single drone, Vallorim is intended to become a reusable engineering platform capable of supporting multiple aircraft configurations and missions over time.



Status: Locked



\---



\# Decision 002 – Aircraft Configuration



Vallorim Mk I will use a conventional fixed-wing electric pusher configuration.



Reason:

A conventional fixed-wing aircraft is significantly less complex than a VTOL aircraft while still providing an excellent platform for learning aircraft design, aerodynamics, flight dynamics, autonomy, and systems engineering. This allows the project to be realistically completed within one year.



Future:

Vallorim Mk II will reuse the same software architecture while introducing VTOL/STOVL capability.



Status: Locked



\---



\# Decision 003 – Mission Role



Vallorim Mk I will function as a modular ISR and autonomy research aircraft.



Primary Mission



• Autonomous Flight

• Reconnaissance

• Onboard Perception

• Mission Planning

• Modular Payload Testing



Design Priorities



1\. Stability

2\. Endurance

3\. Modularity

4\. Easy Simulation

5\. Future AI Integration



Status: Locked



\---



\# Decision 004 – Size Class



Vallorim Mk I will be a small, portable UAV.



Reason:

A portable aircraft is easier to transport, store, manufacture, simulate, and eventually test. It also minimizes regulatory burden while remaining capable of carrying useful sensors and computing hardware.



Initial Targets



Wingspan:

1.2–1.5 m



Takeoff Weight:

Less than 2.5 kg



Payload:

0.25–0.5 kg



Launch:

Hand Launch



Landing:

Belly Landing



Status: Locked



\---



\# Decision 005 – Airframe Layout



Vallorim Mk I will use a high-wing, twin-boom, electric pusher configuration.



Reason:

This layout offers excellent stability, a clear forward field of view for sensors, rear-mounted propulsion for improved payload integration, and a highly modular architecture suitable for ISR and autonomy research.



Design Inspiration



The overall philosophy is inspired by modern ISR aircraft while being scaled for portability and research purposes.



Status: Locked



\---



\# Guiding Philosophy



Build the Platform First.

Expand the Platform Second.



Every subsystem—including CAD, software, avionics, autonomy, payloads, and future aircraft variants—should be designed with modularity and reuse in mind.



The long-term objective is to create a family of autonomous aircraft sharing a common software and systems architecture rather than developing isolated vehicles.

