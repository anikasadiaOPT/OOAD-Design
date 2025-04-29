### Sequence Diagram 
<p> After reading this whole file, we will be able to gain about </p>
    <ul>
      <li> Definition</li>
      <li> Relation to other UML</li>
      <li> Key parts</li>
      <li> Heuristics</li>
      <li> Elements</li>
      <li> Structured Control Operators</li>
      <li> Case Studies</li>
    </ul>

<h2> Definition</h2>
   <uL>
       <li>Interaction</li>
       <li>Detailed operations carried out</li>
       <li>Models Single scenario execution</li>
       <li>models communication behaviour</li>
       <li>Shows Interacting individuals</li>
       <li>Shows message exchange</li>
   </uL>

<h2> Relation to other UML</h2>
    <ul>
        Use case -> Sequence Diagram
    </ul>

<h2>Key parts</h2>
   <uL>
       <li>Frame
           <ul>
               <li>Rectangle with pentagon</li>
               <li>Name Compartment</li>
               <li>Identifier 'sd'</li>
               <li>Simple name or operation specifiation</li>
           </ul>
       </li>
       <li>Participants
        <ul>
            <li>Object or Entity</li>
            <li>Actor/ System</li>
            <li>Rectangle Identifier</li>
        </ul>
       </li>
       <li>Lifelines/Axes
           <uL>
               <li>Participating individuals</li>
               <li>Arrayed across diagram</li>
               <li>Dashed line</li>
               <li>Shows period individuals exists</li>
               <li>Horizontal: Object or participants</li>
               <li>Verticle: Time(time down is forward)</li>
               <li>Creation
                   <ul>New object apperance at creation point</ul>
               </li>
               <li>Destruction
                 <ul>
                     <li>Truncated lifeline</li>
                     <li>Ending in an X</li>
                 </ul>
               </li>
               <li>Persisting Objects</li>
               <li>Identifier format
                  <ul>
                      <li>name[selector]: typeName</li>
                      <li>Name(optional)</li>
                      <li>Selector(optional)</li>
                      <li>TypeName(optional)</li>
                      <li>Name typeName or both must appear</li>
                  </ul>
               </li>
           </uL>
       </li>
       <li>Message
           <ul>
               <li>Communication between participants</li>
               <li>Arrows</li>
               <li>Synchronous
                   <ul>
                       <li>Sender suspends execution</li>
                       <li>Sender waits for reply</li>
                   </ul>
               </li>
               <li>Asynchronous
                   <ul>
                       <li>Sender continues execution</li>
                       <li>No waiting</li>
                   </ul>
               </li>
               <li>Message return</li>
               <li>Object creation</li>
           </ul>
       </li>
       <li>Execution Occurance
           <ul>
               <li>Operation is executing</li>
               <li>Process running code</li>
               <li>Operation suspended(waiting for sync message return)</li>
               <li>Operation active(executing or suspended)</li>
           </ul>
       </li>
       <li>Shown as thin rectangle over lifeline</li>
   </uL>



<h2>Heuristics</h2>

   <ul>
    <li>Sender of first message leftmost</li>
    <li>Heavy interactors next to one another</li>
    <li>Position for short message arrows</li>
    <li>Position for arrows left to right</li>
   </ul>


<h2>Elements</h2>
    <ul>
        <li>Object lifeline(1)</li>
        <li>Message/Stimulus(2)</li>
        <li>Iteration(3)</li>
        <li>Self Reference(4)</li>
        <li>Return(5)</li>
        <li>Anonymus Object(6)</li>
        <li>Object name(7)</li>
        <li>Sequence Number(8)</li>
        <li>Condition(9)</li>
        <li>Basic Comment(10)</li>
        <li>Self Execution(extended)</li>
    </ul>

<h2>Structured Control Operators</h2>

   <ul>
       <li>OPT(optional)</li>
       <li>ALT(Alternate)</li>
       <li>PAR(Parallel)</li>
       <li>Loop(Iterative)</li>
       <li>Ref(Reference)</li>
   </ul>

<h2>Case Studies</h2>
    <ul>
        <li>ATM Withdrawl Machine</li>
        <li>Library Journal Booking</li>
        <li>Hospital Bed/Room Booking</li>
        <li>Air cooler Start Cycle</li>
    </ul>
