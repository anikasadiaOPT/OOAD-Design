# 📘 Class Diagram

After reading this article, you will learn about:

- ✅ What is a Class?
- ✅ Class Diagram Representation
- ✅ Class Diagram Elements
- ✅ Drawing the Class Diagram
- ✅ Class Diagram Relationships
- ✅ Constraints and Notes
- ✅ Logical Distribution of Classes (Packages)
- ✅ Class Categorization
- ✅ CRC Card (Class Responsibility Collaboration)
- ✅ Class vs. Object Diagram
- ✅ References
- ✅ Case Scenarios

---

## 🧠 What is a Class?

A **class** is a blueprint for creating objects that share:

- 🏷️ Similar **properties** (also called **attributes**)
- ⚙️ Common **behavior** (also known as **operations** or **methods**)
- 🔗 Common **relationships** to other objects
- 💡 Common **semantics** (meaning within the system)

### 💡 Examples:
- **Student**
- **Employee**

Each class is a template for creating individual objects (instances).

---

# 🌟 Class Diagram Representation

A **Class Diagram** represents the structure of a system by showing:

- 🧱 **Classes** – Blueprints of objects containing attributes and operations.
- 🧩 **Component Parts** – Attributes (data members) and operations (methods) defining class behavior.
- 🔗 **Relationships Between Classes** – Including association, aggregation, composition, inheritance, and realization.

> 🧠 It’s a foundational diagram in **Object-Oriented Analysis and Design (OOAD)**, helping visualize how different classes interact within the system.

---

## 📚 Class Diagram Elements

### 🧾 Attributes
- **Describe**: Appearance and knowledge of a class.
- **Visibility Modifiers**:
  - `+` **Public** – Accessible from any class.
  - `-` **Private** – Accessible only within the class.
  - `#` **Protected** – Accessible by subclasses.
  - `~` **Package** – Accessible within the same package.
- **Derived Attribute**: Indicated with a slash `/`, computed from other attributes.
- **Attribute Name**:
  - Required
  - Must be unique within a class
  - Should be meaningful (≥3 characters)
- **Data Type**:
  - Required
  - Reflects client view during analysis and language type during design
- **Default Value**:
  - Optional
  - Enhances usability and system integrity
- **Constraints**:
  - Rules to maintain data integrity (e.g., `{ID is assigned by system}`)
- **Static Attribute**:
  - Shared across all instances
  - Underlined in UML (e.g., `__sharedCount: int__`)

---

### ⚙️ Operations (Methods)
- **Describe**: What the object can do.
- **Components**:
  - **Operation Name**: Required (along with parameter list, must be unique within the class)
  - **Arguments / Parameters**:
    - Optional, but each must have:
      - Name (required)
      - Data type (required)
      - Constraints (optional/preconditions)
  - **Return Data Type**:
    - Optional
    - Only one return type allowed (type only, no name)
- **Visibility Modifiers**:
  - `+` Public
  - `-` Private
  - `#` Protected
  - `~` Package

---

### 💠 Stereotypes
- Define the role or type of the class in context (e.g., «boundary», «control», «entity»)

### 🧾 Properties
- Help track maintenance and class definition status.

---

## 🖊️ Drawing the Class Diagram

A class diagram is typically divided into **three compartments**:
- Name Compartments
- Attribute Compartments
- Operation Compartments






---
