# Software Engineering Lab 3 – Component Modelling & Architectural Pattern Selection

## Project: Self-Service Coffee Kiosk System

### 1. Objective
To evaluate different architectural styles, select the most appropriate architecture for the assigned scenario, and create a UML Component Diagram showing system components, interfaces, and dependencies.

### 2. Selected Architecture
**Layered Architecture**

The Self-Service Coffee Kiosk System follows a three-layer architecture:

- **Presentation Layer:** Handles touchscreen interactions and customer selections.
- **Business Layer:** Manages orders, payment processing, and receipt generation.
- **Data Layer:** Stores coffee menu information and pricing details.

### 3. System Components

The system consists of five components:

| Component | Responsibility |
|---|---|
| User Interface Component | Handles touchscreen interactions and coffee selections. |
| Order Manager Component | Manages orders, calculates prices, and coordinates operations. |
| Payment Service Component | Processes credit card payments. |
| Receipt Printer Component | Generates and prints customer receipts. |
| Database Component | Stores coffee types, sizes, menu and pricing information. |

### 4. Interfaces

The following four interfaces connect the system components:

1. **Order Interface:** Connects User Interface and Order Manager.
2. **Payment Interface:** Connects Order Manager and Payment Service.
3. **Receipt Interface:** Connects Order Manager and Receipt Printer.
4. **Database Interface:** Connects Order Manager and Database.

### 5. Functional Requirements

- Customers can select Espresso, Americano, or Latte.
- Customers can choose Small or Large sizes.
- Payments are accepted through credit cards only.
- The system prints receipts containing order details.
- The system stores menu and pricing information.

### 6. Architectural Justification

Layered Architecture was selected because it provides separation of concerns and simplifies component management.

**Security Advantage:** Payment processing is handled separately through the Payment Service Component, supporting secure payment communication.

**Performance Benefit:** Separating application responsibilities allows efficient order processing and menu retrieval.

### 7. Repository Contents

- `Coffee_Kiosk_Component_Diagram.png` – UML Component Diagram.
- `Coffee_Kiosk_Architecture_Justification.pdf` – Written architectural justification.

### 8. Tools Used

- Draw.io (diagrams.net)
- Microsoft Word
- GitHub

---

**Course:** Software Engineering  
**Lab:** Lab 3 – Component Modelling & Architectural Pattern Selection
