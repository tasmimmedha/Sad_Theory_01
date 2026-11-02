# System Analysis and Design (SAD) — Mid Syllabus & Study Notes

> ⚡ **Looking for quick review?** Check [Study_Overview.md](file:///d:/Sad_Theory_01/Study_Overview.md) for 1-line flashcard summaries of all Mid exam topics.

## 📋 Mid Syllabus Overview (Handwritten Notes)

1. **Module 1: Fundamentals of Systems & Software**
   - **1.1 (1)** SDLC & Prototyping
   - **1. (2)** Types of Software
   - **1. (3)** Organization Structure
2. **Module 2: System Planning & Feasibility**
   - **2.1** System Initiation & Scope
   - **2.2 (i)** Types of Feasibility & Applicability to a Scenario
3. **Module 3: System Modeling & Analysis Diagrams**
   - **3.3 (i)** Use Case Diagram *(with `<<include>>` & `<<extend>>`)*
   - **3.3 (ii)** Use Case Descriptive Form
   - **3.3 (iii)** Activity Diagram
   - **3.3 (iv)** Data Flow Diagram (DFD)
   - **3.3 (v)** Swimlane Diagram

---

## 1. Fundamentals of Systems & Software

### 1.1 SDLC & Prototyping

#### A. Software Development Life Cycle (SDLC)
SDLC is a structured process used by systems analysts and developers to plan, design, build, test, and deliver high-quality information systems.

* **1. Planning & Investigation**: Identify problem opportunities, define scope, evaluate project feasibility, and allocate resources.
* **2. Analysis**: Gather business requirements from stakeholders, model current processes, and define requirements for the proposed system (functional vs non-functional).
* **3. Design**: Architectural, logical, and physical system design (UI/UX, database schema, data flows, system interfaces).
* **4. Implementation & Development**: Writing source code, database construction, unit testing, and system integration.
* **5. Testing & Quality Assurance**: Verification and validation against user requirements (integration, system, and user acceptance testing - UAT).
* **6. Deployment & Maintenance**: System installation (direct, parallel, phased, pilot), bug fixes, enhancements, and long-term support.

#### B. Prototyping Model
An iterative development approach where an early working model (prototype) of the system is built, demonstrated to users, and refined based on feedback.

* **Key Steps**:
  1. Identify basic user requirements.
  2. Develop initial working prototype.
  3. User review and feedback collection.
  4. Revise and enhance the prototype.
* **Prototyping Types**:
  * **Throwaway / Rapid Prototyping**: Built quickly to clarify vague requirements and then discarded once requirements are finalized.
  * **Evolutionary Prototyping**: Continuously refined and extended until it becomes the final operational system.
* **Pros & Cons**:
  * *Advantages*: Early user involvement, reduces misunderstanding, clarifies ambiguous requirements.
  * *Disadvantages*: Risk of scope creep, can lead to poor system architecture if rushed, potential user frustration if expectations are unrealistic.

---

### 1.2 Types of Software

1. **System Software**:
   * Serves as the base platform for running hardware and applications.
   * *Examples*: Operating Systems (Windows, Linux, macOS), Device Drivers, BIOS/UEFI, System Utilities.
2. **Application Software**:
   * Designed to help end-users perform specific tasks.
   * **Custom / Bespoke Software**: Tailored to an organization's unique requirements (e.g., custom university portal).
   * **Packaged / Commercial Off-The-Shelf (COTS)**: Readymade software for broad markets (e.g., MS Office, Adobe Suite).
   * **Enterprise Software**: Manages enterprise-wide operations (e.g., ERP systems like SAP, CRM systems like Salesforce).
3. **Embedded Software**:
   * Dedicated software installed directly on non-PC hardware devices with real-time constraints (e.g., automotive controllers, medical devices, IoT sensors).
4. **Web & Cloud-based Software**:
   * Accessible via web browsers and hosted on remote cloud infrastructure (SaaS model) (e.g., Google Workspace, Figma).

---

### 1.3 Organization Structure

Organizational structure dictates how activities are directed, who makes decisions, and how information flows within a company. Systems analysts must design systems that align with the company's structure.

| Structure Type | Characteristics | Impact on System Design |
| :--- | :--- | :--- |
| **Hierarchical / Functional** | Grouped by function/department (HR, Finance, Marketing, Sales). Clear chain of command. | Siloed data stores; often requires departmental reporting and cross-department integration. |
| **Project-Based** | Organized around temporary projects; teams form and disband. | Flexible access controls; collaborative and modular project tracking systems. |
| **Matrix** | Dual reporting lines (functional manager + project manager). | Complex access rules, multi-dimensional approval workflows, and shared resource pools. |
| **Flat / Horizontal** | Few or no middle management levels; direct decision-making. | Decentralized workflows, open data access, and peer-to-peer collaboration tools. |

---

## 2. System Planning & Feasibility Analysis

### 2.1 Feasibility Overview
Feasibility analysis is conducted during the preliminary investigation phase to determine whether an IT project should be pursued, postponed, or rejected.

### 2.2 Types of Feasibility & Applicability to a Scenario

| Feasibility Dimension | Core Questions & Evaluation Focus | Scenario Application Checklist |
| :--- | :--- | :--- |
| **1. Technical Feasibility** | *Can we build it?*<br>• Availability of required hardware, software, and tools.<br>• Technical competence and team expertise.<br>• System scalability and integration with legacy systems. | Analyze current infrastructure, assess team skillset vs tech stack learning curve, verify compatibility. |
| **2. Economic Feasibility** | *Does it make business sense?*<br>• Cost-Benefit Analysis (CBA).<br>• Tangible costs (development, hardware) vs intangible costs (operational disruption).<br>• Tangible benefits (cost reduction) vs intangible benefits (customer satisfaction).<br>• ROI (Return on Investment) and Payback Period. | Calculate total cost of ownership (TCO), compare expected cash inflows/savings against costs. |
| **3. Operational Feasibility** | *Will it be used effectively?*<br>• User acceptance and resistance to change.<br>• Fit with existing organizational culture and standard operating procedures (SOPs).<br>• Training and support requirements. | Survey user willingness, evaluate workflow impact, design change-management plans. |
| **4. Schedule / Time Feasibility** | *Can it be delivered in time?*<br>• Critical deadlines (regulatory dates, market windows).<br>• Resource constraints and realistic milestone estimates. | Review Gantt charts, check for tight market deadlines, evaluate delivery risks. |
| **5. Legal & Ethical Feasibility** | *Is it legally permissible?*<br>• Data privacy laws (GDPR, local regulations).<br>• Copyright, intellectual property, contracts, licensing, and compliance. | Ensure user data compliance, audit software licenses, verify legal liability. |

#### 💡 Scenario Applicability Example:
> **Exam Scenario**: *"A private clinic wants to transition from paper records to a cloud-based Electronic Health Record (EHR) system within 3 months with a limited budget and staff with low computer literacy."*
> - **Technical**: High (cloud EHR tools exist, but clinic internet reliability must be verified).
> - **Economic**: Moderate (cloud subscriptions reduce upfront cost, but recurring subscription & setup fees must fit budget).
> - **Operational**: Critical Risk (staff resistance and low digital literacy require extensive training).
> - **Schedule**: High Risk (3 months is extremely tight for transition, data entry, and training).
> - **Legal**: High Importance (strict compliance required for patient medical data confidentiality).

---

## 3. System Modeling & Analysis Diagrams

### 3.3 (i) Use Case Diagram (with `<<include>>` & `<<extend>>`)

* **Purpose**: Captures system functional requirements from the perspective of external users (Actors).
* **Core Components**:
  * **System Boundary**: Rectangle representing the scope of the system.
  * **Actor**: Stick figure representing human roles, external systems, or time triggers interacting with the system.
  * **Use Case**: Horizontal ellipse representing a distinct functional goal (e.g., `Make Payment`).
  * **Association**: Solid line connecting an Actor to a Use Case.

#### Key Relationships:
1. **`<<include>>` (Mandatory / Common Functionality)**:
   * The base use case **always** executes the included use case.
   * Used for common behavior shared by multiple use cases.
   * *Direction*: Arrow points from Base Use Case $\rightarrow$ Included Use Case.
   * *Example*: `Place Order` $-\!-\!-\!-\!-\!\gg$ `<<include>>` $\rightarrow$ `Verify Inventory`.
2. **`<<extend>>` (Optional / Conditional Behavior)**:
   * The extending use case executes **only under certain conditions** (extension points).
   * Used to handle optional steps, error conditions, or special features.
   * *Direction*: Arrow points from Extending Use Case $\rightarrow$ Base Use Case.
   * *Example*: `Apply Discount Coupon` $-\!-\!-\!-\!-\!\gg$ `<<extend>>` $\rightarrow$ `Checkout Cart`.

---

### 3.3 (ii) Use Case Descriptive Form

A standardized textual specification detailing each use case:

| Field | Description / Example |
| :--- | :--- |
| **Use Case ID & Name** | UC-01: User Login |
| **Primary Actor** | Registered Customer |
| **Stakeholders & Interests** | Customer (quick access), Security Team (prevent unauthorized access) |
| **Preconditions** | User must have an active registered account |
| **Postconditions** | User is authenticated and redirected to dashboard |
| **Trigger** | User navigates to the login page and enters credentials |
| **Main Success Scenario (Happy Path)** | 1. User enters username and password.<br>2. System validates credentials.<br>3. System establishes user session.<br>4. System displays dashboard. |
| **Alternative Flows** | 2a. User selects "Remember Me": system issues persistent token. |
| **Exception Flows** | 2b. Invalid credentials: system shows error message and prompts password reset. |

---

### 3.3 (iii) Activity Diagram

* **Purpose**: Models procedural flows, business workflows, and operational step-by-step logic.
* **Notation**:
  * **Initial Node**: Filled black circle (●).
  * **Activity / Action**: Rounded rectangle.
  * **Control Flow**: Directed arrow showing sequence.
  * **Decision Node**: Diamond with incoming arrow and multiple outgoing guarded branches `[condition]`.
  * **Merge Node**: Diamond bringing alternative paths back together.
  * **Fork & Join**: Horizontal/vertical thick black bar used for concurrent/parallel activities.
    * *Fork*: 1 incoming flow $\rightarrow$ multiple parallel outgoing flows.
    * *Join*: Multiple parallel incoming flows $\rightarrow$ 1 synchronized outgoing flow.
  * **Final Node**: Bullseye / bordered circle (◉).

---

### 3.3 (iv) Data Flow Diagram (DFD)

* **Purpose**: Illustrates how data moves through a system, where it is transformed, stored, and routed.
* **Basic Symbols (Gane & Sarson / Yourdon)**:
  * **External Entity (Source / Sink)**: Rectangle. Entities outside the system supplying or receiving data.
  * **Process**: Rounded rectangle / circle. Transforms inputs into outputs (labeled with a verb-noun phrase, e.g., `Calculate Invoice`).
  * **Data Store**: Open-ended rectangle / two parallel horizontal lines. Represents data at rest (database, file).
  * **Data Flow**: Labeled directed arrow showing movement of data packets.
* **DFD Hierarchy**:
  * **Context Diagram (Level 0)**: High-level view showing the entire system as a single process with external entities and major inputs/outputs.
  * **Level 1 DFD**: Decomposes the single system process into major sub-processes, showing internal data stores.
  * **Level 2 DFD**: Further decomposes complex Level 1 sub-processes into detailed steps.

---

### 3.3 (v) Swimlane Diagram

* **Purpose**: A cross-functional activity or process diagram partitioned into columns or rows ("lanes").
* **Key Concept**:
  * Each lane represents an organizational department, user role (e.g., Customer, Sales, Accounting, Warehouse), or system subsystem.
  * Shows **who** is responsible for **what** step in a workflow.
  * Clearly highlights handoffs, bottlenecks, and cross-department dependencies.
