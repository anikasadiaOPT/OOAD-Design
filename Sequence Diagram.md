<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sequence Diagram</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 30px;
      line-height: 1.6;
      background-color: #f9f9f9;
      color: #333;
    }
    h1, h2 {
      color: #2c3e50;
    }
    ul {
      margin-left: 20px;
    }
    li {
      margin-bottom: 5px;
    }
    .section {
      margin-bottom: 30px;
      padding: 20px;
      background-color: #ffffff;
      border-left: 5px solid #2980b9;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
  </style>
</head>
<body>

  <h1>Sequence Diagram</h1>

  <p>After reading this guide, you will understand the following:</p>
  <ul>
    <li>Definition</li>
    <li>Relation to other UML Diagrams</li>
    <li>Key Parts</li>
    <li>Heuristics</li>
    <li>Elements</li>
    <li>Structured Control Operators</li>
    <li>Case Studies</li>
  </ul>

  <div class="section">
    <h2>Definition</h2>
    <ul>
      <li>Represents interaction among objects</li>
      <li>Shows detailed operations carried out</li>
      <li>Models a single scenario execution</li>
      <li>Depicts communication behavior</li>
      <li>Highlights interacting individuals</li>
      <li>Displays message exchange</li>
    </ul>
  </div>

  <div class="section">
    <h2>Relation to Other UML Diagrams</h2>
    <ul>
      <li><strong>Use Case</strong> → <strong>Sequence Diagram</strong></li>
    </ul>
  </div>

  <div class="section">
    <h2>Key Parts</h2>
    <ul>
      <li><strong>Frame</strong>
        <ul>
          <li>Rectangle with a pentagon corner</li>
          <li>Includes a name compartment</li>
          <li>Identifier: <code>sd</code></li>
          <li>Simple name or operation specification</li>
        </ul>
      </li>
      <li><strong>Participants</strong>
        <ul>
          <li>Objects or entities</li>
          <li>Actors or system components</li>
          <li>Represented using rectangle identifiers</li>
        </ul>
      </li>
      <li><strong>Lifelines / Axes</strong>
        <ul>
          <li>Represent participating individuals</li>
          <li>Dashed vertical lines across the diagram</li>
          <li>Show the lifetime of participants</li>
          <li><strong>Horizontal axis</strong>: participants</li>
          <li><strong>Vertical axis</strong>: time (flows downward)</li>
          <li><strong>Creation</strong>: New object appears at creation point</li>
          <li><strong>Destruction</strong>: Ends with an 'X' symbol</li>
          <li><strong>Identifier Format</strong>: <code>name[selector]: typeName</code></li>
        </ul>
      </li>
      <li><strong>Message</strong>
        <ul>
          <li>Arrows representing communication</li>
          <li><strong>Synchronous</strong>: Sender waits for a reply</li>
          <li><strong>Asynchronous</strong>: Sender continues without waiting</li>
          <li>Includes message return and object creation</li>
        </ul>
      </li>
      <li><strong>Execution Occurrence</strong>
        <ul>
          <li>Indicates operation execution</li>
          <li>Process may be active or waiting</li>
          <li>Shown as a thin rectangle over the lifeline</li>
        </ul>
      </li>
    </ul>
  </div>

  <div class="section">
    <h2>Heuristics</h2>
    <ul>
      <li>Sender of the first message should be on the left</li>
      <li>Heavy interactors placed close together</li>
      <li>Keep message arrows short</li>
      <li>Prefer left-to-right arrow direction</li>
    </ul>
  </div>

  <div class="section">
    <h2>Elements</h2>
    <ul>
      <li>Object Lifeline</li>
      <li>Message / Stimulus</li>
      <li>Iteration</li>
      <li>Self-Reference</li>
      <li>Return</li>
      <li>Anonymous Object</li>
      <li>Object Name</li>
      <li>Sequence Number</li>
      <li>Condition</li>
      <li>Basic Comment</li>
      <li>Self Execution (extended)</li>
    </ul>
  </div>

  <div class="section">
    <h2>Structured Control Operators</h2>
    <ul>
      <li><strong>opt</strong> – Optional</li>
      <li><strong>alt</strong> – Alternative paths</li>
      <li><strong>par</strong> – Parallel execution</li>
      <li><strong>loop</strong> – Iterative execution</li>
      <li><strong>ref</strong> – Reference another interaction</li>
    </ul>
  </div>

  <div class="section">
    <h2>Case Studies</h2>
    <ul>
      <li>ATM Withdrawal Machine</li>
      <li>Library Journal Booking</li>
      <li>Hospital Bed/Room Booking</li>
      <li>Air Cooler Start Cycle</li>
    </ul>
  </div>

</body>
</html>
