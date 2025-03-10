# practical1
Vehicle mangament system
# Vehicle Management System

# Vehicle Management System

## Objectives
After completing this project, you will be able to:

- Identify ambiguities, inconsistencies, and incompleteness in a requirements specification.
- Identify and state functional requirements.
- Identify and state non-functional requirements.

## Time Required
Approximately 3 hours

## Requirements
Sommerville defines a "requirement" as a specification of what should be implemented. Requirements specify how the target system should behave, defining **what to do** but not **how to do it**.

Requirements engineering refers to the process of understanding what a customer expects from the system to be developed and documenting them in a standard, easily readable, and understandable format. This document serves as a reference for the subsequent design, implementation, and verification of the system.

Before starting the planning, design, and implementation of the **Vehicle Management System**, it is crucial to have a clear understanding of its requirements. A lack of clarity can lead to serious issues and customer dissatisfaction.

## Characteristics of Requirements
Requirements gathered for the **Vehicle Management System** should exhibit the following properties:

- **Unambiguity**: The system requirements should be clear and unambiguous. For example, if a requirement states that the system should handle "many" vehicles, it should specify the exact number or range to avoid misinterpretation.
- **Consistency**: The requirements should not contradict each other. For example, if one requirement states that a vehicle can be rented for a maximum of 7 days, another requirement should not state that it can be rented for 10 days.
- **Completeness**: Requirements should specify both **what the system should do** and **what it should not do**. For example, if a vehicle is already booked, the system should notify the user and prevent duplicate bookings.

## Categorization of Requirements
### Based on the Target Audience
- **User Requirements**: Written in natural language for easy understanding by customers.
- **System Requirements**: Written using technical terms meant for development and testing teams.

### Based on What They Describe
#### Functional Requirements (FRs)
These define how the system should react to a particular set of inputs and what outputs it should produce. Some functional requirements for the **Vehicle Management System** include:

- The system should allow users to register and log in.
- Users should be able to add, update, and delete vehicle records.
- The system should allow users to book a vehicle for a specified period.
- Users should be able to track vehicle availability in real time.
- The system should generate billing invoices after rental completion.
- The system should support vehicle maintenance tracking.
- The system should manage driver assignments for vehicles.
- Inventory items required for maintenance should be recorded and tracked.

#### Non-Functional Requirements (NFRs)
These describe constraints and behaviors of the system under certain conditions. Examples include:

- **Product Requirements**: The system should have a user-friendly web interface with a mobile-friendly design.
- **Performance Requirements**: The system should handle up to 1,000 concurrent users.
- **Organizational Requirements**: The development process should comply with Agile methodology and industry standards.

## Entity-Relationship (ER) Diagram Details
The **Vehicle Management System** consists of several entities and their relationships:

### **Entities and Attributes**
# Vehicle Management System

## Entities and Attributes

### Vehicle
- **Registration Number** (Primary Key)
- **Model**
- **Type** (Car, Truck, Bus, etc.)
- **Fuel Type** (Petrol, Diesel, Electric, etc.)
- **Usage Status** (Active, In Maintenance, Decommissioned)

### Driver
- **Driver ID** (Primary Key)
- **Name**
- **Badge Number**
- **Age**
- **Assigned Vehicle** (Foreign Key - Relationship: A driver is assigned to one vehicle)

### Mechanic
- **Mechanic ID** (Primary Key)
- **Name**
- **Rank**
- **Specialization** (Engine, Transmission, Electrical, etc.)
- **Assigned Vehicles** (Foreign Key - Relationship: A mechanic can be responsible for multiple vehicles)

### Maintenance
- **Work Order ID** (Primary Key)
- **Vehicle Registration Number** (Foreign Key - Relationship: A work order is linked to a specific vehicle)
- **Mechanic Assigned** (Foreign Key - Relationship: A work order is assigned to a specific mechanic)
- **Maintenance Type** (Routine, Repair, Emergency, etc.)
- **Status** (Pending, In Progress, Completed)

### Inventory
- **Item ID** (Primary Key)
- **Item Name**
- **Quantity Available**
- **Used in Maintenance** (Foreign Key - Relationship: Inventory items are used for specific maintenance tasks)

### Checks
- **Check ID** (Primary Key)
- **Performed by Mechanic** (Foreign Key - Relationship: Checks are performed by mechanics)
- **Associated with a Vehicle** (Foreign Key - Relationship: Checks are conducted on specific vehicles)
- **Inspection Date**
- **Status** (Passed, Failed, Requires Attention)

## Relationships
1. **A vehicle is assigned to one driver, but a driver can have only one active vehicle at a time.**
2. **A mechanic is responsible for multiple vehicles.**
3. **A maintenance work order is linked to both a specific vehicle and a mechanic.**
4. **Inventory items are consumed during maintenance.**
5. **Mechanics perform routine checks on vehicles, which determine their maintenance needs.**

This refined structure ensures clarity, normalization, and proper entity relationships within the Vehicle Management System. 🚗🔧📋



## Identifying Functional Requirements
To identify functional requirements for the **Vehicle Management System**, consider the following:

1. **High-Level Functionalities**:
   - Vehicle registration
   - Rental booking
   - Vehicle tracking
   - Payment processing
   - Report generation
   - Maintenance tracking
   - Driver assignments
   - Inventory management

2. **User-Centric Approach**:
   - A registered user should be able to search for available vehicles.
   - The system should notify users of upcoming rental expiration.
   - Admins should have access to manage vehicle records and maintenance schedules.

3. **System as a Black Box**:
   - Inputs: User selects a vehicle and rental duration.
   - Outputs: The system provides vehicle availability, rental confirmation, and an invoice.

4. **Sub-requirements**:
   - "Book a Vehicle" may have different conditions based on vehicle type, availability, and user membership level.

## Preparing the Software Requirements Specification (SRS)
Once all functional and non-functional requirements are identified, an **SRS document** should be prepared. IEEE provides a standard template for SRS documentation. The **SRS serves as a legal agreement** between the client and the service provider. If a feature is missing post-development, the client can refer to the SRS. Likewise, new features requested after project completion must be negotiated separately if not listed in the SRS.

While this README does not cover writing an SRS, it outlines the foundational aspects of requirements engineering necessary for a successful **Vehicle Management System**.

