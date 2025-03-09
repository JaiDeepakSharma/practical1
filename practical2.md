# Vehicle Management System  Practical 2- Project Estimation

## Introduction
The Vehicle Management System (VMS) is designed to facilitate the efficient management of vehicles, drivers, mechanics, and maintenance activities within an organization. The system will enable vehicle tracking, assignment to drivers, maintenance scheduling, and inventory management for vehicle-related parts. The final deliverable is a **web-based application** that will run within the organization's secure intranet, ensuring data privacy and controlled access.

Given the complexity and scope of the project, **COCOMO (Constructive Cost Model)** is used for project estimation. Based on the team size (small) and experience level (high), the project is categorized as an **"organic"** software development effort.

---

## Project Estimation Using Basic COCOMO

The COCOMO model estimates the effort, cost, and time required for project completion based on **KLOC (Kilo Lines of Code)**.

### Formula:
Effort (PM) = **a * (KLOC)^b**

Tdev (Months) = **2.5 * (Effort)^c**

For an **organic** project, the standard parameter values are:
- **a = 2.4**
- **b = 1.05**
- **c = 0.38**

#### Estimated Size of Vehicle Management System
Based on prior experience with similar systems, the estimated size of the **VMS software** is **12 KLOC**.

### Effort Calculation:
Effort = 2.4 * (12)^1.05
       ≈ 32.2 PM (Person-Months)

### Development Time Calculation:
Tdev = 2.5 * (32.2)^0.38
     ≈ 9.1 months

Thus, based on the **basic COCOMO model**, the estimated effort required is **32.2 person-months**, and the project is expected to be completed in **9 months**.

---

## Refinement Using Intermediate COCOMO

Intermediate COCOMO considers **Effort Adjustment Factors (EAF)** based on product attributes, hardware attributes, personnel capabilities, and project requirements.

### Cost Driver Ratings:
| Cost Driver | Chosen Rating | Value |
|-------------|---------------|-------|
| Required software reliability | Nominal | 1.00 |
| Size of application database | Nominal | 1.00 |
| Complexity of the product | High | 1.15 |
| Run-time performance constraints | Nominal | 1.00 |
| Memory constraints | Nominal | 1.00 |
| Volatility of virtual machine environment | Nominal | 1.00 |
| Required turnabout time | Low | 0.87 |
| Analyst capability | High | 0.86 |
| Applications experience | High | 0.91 |
| Software engineer capability | High | 0.86 |
| Virtual machine experience | Nominal | 1.00 |
| Programming language experience | Nominal | 1.00 |
| Application of software engineering methods | High | 0.91 |
| Use of software tools | High | 0.91 |
| Required development schedule | High | 1.04 |

### Effort Adjustment Factor (EAF):
EAF = **0.55 (approx)** (product of all chosen rating values)

Using this EAF value, the refined estimates are:

### Corrected Effort Calculation:
Effort|corrected = 32.2 * 0.55
                 ≈ 17.7 PM

### Corrected Development Time Calculation:
Tdev|corrected = 2.5 * (17.7)^0.38
               ≈ 7.5 months

Thus, after applying **Intermediate COCOMO adjustments**, the expected effort is **17.7 person-months**, and the project completion time is **7.5 months**.

---

## Final Considerations
- The **basic COCOMO model** estimated **9 months**, but with refined **intermediate COCOMO**, the project is likely to be completed within **7.5 months**.
- The estimation does **not** account for external factors such as requirement changes, scope creep, or unforeseen delays.
- If additional complexities arise, a **Complete COCOMO model** can further refine the estimation based on subsystem components.

This refined estimation ensures better accuracy in planning and resource allocation for the Vehicle Management System. 🚗📊


