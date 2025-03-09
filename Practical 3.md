# Modeling UML Use Case Diagrams and Capturing Use Case Scenarios

## Introduction
Use Case modeling helps in defining the system's functional requirements and interactions between various entities. For the **Vehicle Management System (VMS)**, Use Case Diagrams illustrate how different actors interact with the system.

---

## Key Concepts

### 1. Use Case Diagram Elements
- **Actor**: Represents a user or another system that interacts with VMS.
- **Use Case**: A function or service provided by VMS.
- **Subject**: The boundary that defines the scope of the system.
- **Graphical Representation**: A UML diagram showcasing the interactions.
- **Association**: The link between an actor and a use case.

### 2. Use Case Relationships
- **Include Relationship**: Represents a mandatory dependency between use cases.
- **Extend Relationship**: Represents an optional dependency triggered under specific conditions.
- **Generalization Relationship**: Represents a hierarchy where specialized use cases inherit from general ones.

---

## Identifying Actors
| Actor | Description |
|--------|-------------|
| **Admin** | Manages vehicle records, assigns drivers, and oversees system operations. |
| **Driver** | Uses assigned vehicles and updates trip logs. |
| **Mechanic** | Performs maintenance and updates repair records. |
| **Inventory Manager** | Manages spare parts and maintenance supplies. |
| **User (Employee/Customer)** | Can request a vehicle or check availability. |

---

## Identifying Use Cases
| Use Case | Description |
|-----------|----------------|
| UC1. Register User | Allows a new user (driver, mechanic, admin) to register in the system. |
| UC2. User Login | Authenticates a user based on credentials. |
| UC3. Add Vehicle | Allows an admin to register a new vehicle. |
| UC4. Assign Vehicle | Enables an admin to assign a vehicle to a driver. |
| UC5. Update Maintenance Record | A mechanic logs maintenance activities. |
| UC6. Track Vehicle | Allows real-time vehicle tracking. |
| UC7. Request Vehicle | An employee requests a vehicle for official use. |
| UC8. Approve Vehicle Request | Admin approves/rejects a vehicle request. |

---

## Use Case Relationships
- **Include Relationship**
  - "UC5: Update Maintenance Record" includes **Verify Vehicle Status** before logging a repair.
- **Extend Relationship**
  - "UC7: Request Vehicle" extends **UC8: Approve Vehicle Request** if approval is required.
- **Generalization Relationship**
  - "Assign Vehicle" generalizes into **Assign Temporary Vehicle** or **Assign Permanent Vehicle**.

---

## Guidelines for Drawing Use Case Diagrams
1. **Identify all actors** interacting with the system.
2. **Define system boundaries** (VMS functions vs. external interactions).
3. **List all use cases** and their relationships.
4. **Use UML notation** for **include, extend, and generalization relationships**.
5. **Keep it simple** and understandable.

---

## Conclusion
Use Case modeling provides a structured approach to understanding system functionalities and actor interactions. The **Vehicle Management System (VMS)** use case diagram ensures efficient system design, clarity in requirements, and seamless development. 🚗📊

