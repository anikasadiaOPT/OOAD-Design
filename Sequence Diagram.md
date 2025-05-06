# 📊 Sequence Diagram

After reading this document, you will gain knowledge about:

* ✅ Definition
* 🔄 Relation to other UML diagrams
* 🧩 Key Parts
* 🧠 Heuristics
* 🧱 Elements
* 🔁 Structured Control Operators
* 📚 Case Studies

---

## 📘 Definition

Sequence diagrams are used to:

* Model **interactions** between objects or entities
* Show **detailed operations** carried out
* Represent a **single scenario execution**
* Illustrate **communication behavior**
* Display **interacting individuals**
* Show **message exchanges** between participants

---

## 🔗 Relation to Other UML Diagrams

* **Use Case** ➡️ **Sequence Diagram**

Sequence diagrams are typically derived from use cases to visually model the sequence of operations.

---

## 🔍 Key Parts

### 📐 Frame

* Rectangle with a pentagon at the top-left
* Includes a **name compartment**
* Identified using **`sd`** keyword
* Contains a **simple name** or **operation specification**

### 👤 Participants

* Represents an **Object** or **Entity**
* Can be an **Actor** or **System**
* Shown as a **rectangle** with identifier

### 📈 Lifelines / Axes

* Represent **participating individuals**
* Arranged **horizontally** across the diagram
* Shown as **dashed vertical lines**
* Indicate **time** (top to bottom → forward in time)
* **Creation**: Object appears at its creation point
* **Destruction**: Lifeline ends with an 'X'
* **Persisting objects** remain active throughout

#### Identifier Format:

```
name[selector]: typeName
```

* `name` (optional)
* `selector` (optional)
* `typeName` (optional)
* At least `name` or `typeName` must appear

### 🔁 Messages

* Show **communication** between participants
* Represented as **arrows**
* Types:

  * **Synchronous**:

    * Sender suspends execution
    * Waits for a reply
  * **Asynchronous**:

    * Sender continues execution
    * Does not wait for a reply
  * **Return Message**
  * **Object Creation**

### ⚙️ Execution Occurrence

* Represents code execution
* Can be:

  * Actively executing
  * Suspended (waiting for return)
* Displayed as a **thin rectangle** over the lifeline

---

## 💡 Heuristics

* Place **sender of the first message** at the **leftmost**
* Keep **heavily interacting objects** close together
* Ensure **short message arrows**
* Prefer **left-to-right** message flow

---

## 🧱 Elements

1. Object Lifeline
2. Message / Stimulus
3. Iteration
4. Self Reference
5. Return
6. Anonymous Object
7. Object Name
8. Sequence Number
9. Condition
10. Basic Comment
11. Self Execution (extended)

---

## 🧭 Structured Control Operators

* `opt` — Optional
* `alt` — Alternate (if-else)
* `par` — Parallel execution
* `loop` — Iteration
* `ref` — Reference to another sequence diagram

---

## 📚 Case Studies

* 🏧 ATM Withdrawal Machine
* 📖 Library Journal Booking
* 🏥 Hospital Bed/Room Booking
* ❄️ Air Cooler Start Cycle
