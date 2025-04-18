🧱 Practical 7: Modeling UML Class Diagrams and Sequence Diagrams
🎯 Aim
To model the object-oriented design of the Motor Transport System using Class Diagrams and Sequence Diagrams.
________________________________________
📘 Introduction
Class diagrams depict the static structure of the system, while Sequence diagrams show how objects interact over time through message passing.
________________________________________
📚 Theory
•	🧩 Class Diagram:
o	Classes with attributes and methods
o	Relationships: Association, Inheritance, Aggregation
•	🕒 Sequence Diagram:
o	Lifelines represent objects
o	Arrows show messages (function calls)
o	Time flows from top to bottom
________________________________________
🧪 Case Study: Motor Transport Section
📌 Class Diagram
•	Class: Vehicle, Driver, Request, Trip, Admin
•	Attributes: licenseNo, fuelLevel, requestDate
•	Methods: assign(), schedule(), approve()
📌 Sequence Diagram (Use Case: Assign Vehicle)
•	Requester → TransportOfficer: RequestVehicle()
•	TransportOfficer → System: validateRequest()
•	System → Vehicle: checkAvailability()
•	TransportOfficer → Driver: assignTrip()
________________________________________
✅ Conclusion
These diagrams help in creating modular, reusable, and maintainable software. They also bridge the gap between requirement analysis and implementation.

