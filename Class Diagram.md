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


# 📘 Class Diagram Relationships

## 🔗 Association
- A **semantic and structural relationship** between classes.
- **Objects recognize** each other and may send messages.
- Can include:
  - **Association name** (should be a verb or verb phrase)
  - **Role names** (nouns representing each end)
  - **Multiplicity** (e.g., 1, 0..*, 1..*)
  - **Navigability** (direction of access)
- **Types of Associations**:
  - Simple
  - Aggregate
  - Composite
  - Reflexive (self-relationship)
  - Qualified (uses an index/qualifier)

## 🔘 Association Class
- Encapsulates **extra information** about an association.

---

## 🔷 Aggregation
- Represents a **"whole-part"** (has-a) relationship.
- The **part can exist independently** of the whole.
- Example: A *Team* has *Players* – players can exist without the team.

---

## 🔶 Composition
- A **strong form of aggregation**.
- The **whole owns the part exclusively**.
- The **part's lifetime depends** on the whole.
- If the whole is deleted, so is the part.
- Example: A *House* contains *Rooms* – if the house is destroyed, rooms are too.

---

## 🧬 Generalization (Inheritance)
- Relationship between a **general (super) class** and **specific (sub) class**.
- Follows the **substitutability principle**.
- A **bottom-up process** ("is-a-kind-of" relationship).
- A subclass:
  - **Inherits** attributes, operations, relationships.
  - **May add or override** features.
- Superclass may be declared `{abstract}` if no instances are created.

---

## 🎭 Realization
- Indicates that a **class implements an interface**.
- A class may **realize many interfaces**.
- Interfaces define **behavior contracts**, not implementation.

---

## ⚠️ Dependency
- A **semantic relationship**.
- A **change in one class may require changes** in the other.
- Indicates **temporary usage** (e.g., within a method).

---

> ✅ Suitable for: UML class diagrams, design documentation, and object-oriented analysis.












---
