# What is a System? — System Analysis and Design (SAD)

> 📌 **Overview**: A fundamental concept in System Analysis and Design (SAD). Understanding what constitutes a system, its components, characteristics, and classifications provides the foundation for analyzing, modeling, and designing modern information systems.

---

## 1. Definition of a System

* The word **"System"** originates from the Greek word *synistêmi*, meaning *"to place together"* or *"an organized whole"*.
* **Formal Definition**: A system is an organized collection of interrelated and interdependent components (subsystems) that work together according to a plan or set of rules to achieve a common goal or objective.

$$ \text{System} = \text{Components} + \text{Interrelationships} + \text{Shared Objective} $$

---

## 2. Core Elements of a System

Every system operates through a continuous cycle of inputs, processing, outputs, and feedback:

```
                  ┌────────────────────────┐
                  │      Environment       │
                  │                        │
  ┌───────┐       │   ┌────────────────┐   │       ┌────────┐
  │ Input │ ────> │   │   Processing   │   │ ────> │ Output │
  └───────┘       │   │ (Transformation│   │       └────────┘
                  │   └────────────────┘   │
                  │           │            │
                  │           ▼            │
                  │   ┌────────────────┐   │
                  │   │Control/Feedback│   │
                  │   └────────────────┘   │
                  │      System Boundary   │
                  └────────────────────────┘
```

1. **Inputs**: The raw data, energy, resources, or requests entering the system from the environment.
2. **Processing (Transformation)**: The internal algorithms, business logic, calculations, and operations that transform inputs into meaningful results.
3. **Outputs**: The finished products, services, or processed information delivered back to users or the external environment.
4. **Feedback**: Output information recycled back into the system to measure actual performance against desired standards.
5. **Control**: The decision-making mechanism that evaluates feedback and applies corrective actions to keep the system on course.
6. **Boundary**: The perimeter that defines the scope of the system and separates it from the external environment.
7. **Environment**: Everything outside the system boundary that influences or is influenced by the system (e.g., vendors, customers, government regulations).
8. **Interfaces**: Designated interaction points where data and energy cross between the system boundary and external entities.

---

## 3. Key Characteristics of a System

| Characteristic | Description | SAD Implication |
| :--- | :--- | :--- |
| **Organization (Structure)** | Structure and order; components are arranged in a specific hierarchy rather than randomly. | Dictates architecture, workflows, and module layering. |
| **Interaction** | Components communicate with and affect one another via defined interfaces. | Requires standardized communication protocols and data exchange formats. |
| **Interdependence** | Subsystems depend on one another; output of one subsystem is frequently the input to another. | Failure in one component can cascade if error-handling and decoupling are absent. |
| **Integration** | All components collaborate harmoniously to fulfill the overall objective rather than individual sub-goals. | Avoids local optimization that harms global system performance. |
| **Central Objective** | Every system exists to serve a predefined business, operational, or technical goal. | System requirements must align with organizational strategy. |

---

## 4. Classification / Types of Systems

### A. Physical vs. Abstract Systems
* **Physical Systems**: Tangible, concrete entities that can be touched and observed (e.g., computer hardware, automated assembly line, desk).
* **Abstract (Conceptual) Systems**: Intangible concepts, mathematical models, equations, or organizational policies (e.g., economic models, software algorithms).

### B. Open vs. Closed Systems
* **Open System**: Continuously interacts with, adapts to, and exchanges information/energy with its external environment (e.g., modern web apps, businesses, biological organisms). *All real-world information systems are open systems.*
* **Closed System**: Completely isolated from its environment; neither inputs nor outputs cross its boundary (e.g., a sealed chemical reaction in a vacuum, pure theoretical models).

### C. Deterministic vs. Probabilistic Systems
* **Deterministic System**: Operates in a completely predictable manner; a given set of inputs always produces the exact same output (e.g., a compiler, automated calculator).
* **Probabilistic System**: Subject to uncertainty; behavior can only be stated in terms of probabilities (e.g., stock market prediction system, weather forecasting).

### D. Man-made (Human-made) vs. Natural Systems
* **Natural Systems**: Naturally occurring systems not created by humans (e.g., solar system, human nervous system, water cycle).
* **Man-made Systems**: Systems designed and built by humans to meet specific needs (e.g., ERP systems, transportation networks, telecommunication networks).

---

## 5. What is an Information System (IS)?

In System Analysis and Design, our primary focus is on **Computer-Based Information Systems (CBIS)**:

> **Information System**: An integrated set of components for collecting, storing, processing, and communicating data to provide information for decision-making, coordination, and control.

### The 5 Essential Pillars of an Information System:
1. **Hardware**: Physical devices (servers, clients, storage drives, networking gear).
2. **Software**: Programs and operating systems that instruct hardware (OS, database management systems, application apps).
3. **Data**: Raw facts and figures stored in databases and file systems awaiting processing.
4. **Procedures / Processes**: Operational rules, policies, and instructions governing how system tasks are executed.
5. **People**: End-users, systems analysts, developers, database administrators, and managers who interact with the system.

---

## 6. System Decomposition: Subsystems & Modularity

Complex systems are broken down into smaller, manageable units called **Subsystems**:
* **Decomposition**: Dividing a system into hierarchical levels of subsystems to reduce complexity and allow independent analysis.
* **Cohesion**: The degree to which elements within a single subsystem belong together (aim for **high cohesion**).
* **Coupling**: The degree of interdependence between different subsystems (aim for **loose coupling**).

---

## ⚡ Quick Flashcard Summary
* **What is a System?** An organized set of interdependent components interacting to achieve a common goal.
* **Basic Cycle**: `Input -> Processing -> Output` regulated by `Feedback & Control`.
* **Real-world IS**: Always an **open, man-made, physical/abstract, probabilistic/deterministic** system built from hardware, software, data, procedures, and people.
