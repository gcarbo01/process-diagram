# process-diagram
<br>

##
<img src="./images/process-diagram-main.jpg" align="center" width=75% height=75%>

##

<br>
<br>
<br>

## Intro
### Summary
In large programs, the business process is the best artefact that can be used to describe the functionality, scope, actors and functional permutations. Consequently, the Architects receive these business processes as input for business requirements. <br> 
Sometimes, Architects need help reading these processes because they are not detailed or granular requirements. Because they are not documented in a way that can transform them into functional and Systema requirements straightaway. So, the Architects need to collaborate with the Business analysts to understand these diagrams and transform them into business and system requirements. <br> 
These business processes are created with different styles, and usually, there is no unity in notation and granularity if more than one business analyst works on them.  Sometimes business analysts have different skills and opinions on how much detail these diagrams should have.  Some business analysts may use a high-level approach to describe the business flows. On other occasions, they may use detailed notations to describe business logic. <br> 
This article discusses the several options for using the notations available in the swimlane process diagrams and the activity diagrams and how these correlate to the design of solutions architecture, applications, and the consequent definition of the agile process artefacts such as epics and user stories.  <br> 
If the process diagrams are too high level, do not show all the actors involved, or do not show enough details for architects to use as input, it could require that the process diagrams be further refined and clarified before actually being useful for architecture input.  <br> 
Discussing the purpose and the motivation of defining which standards to use when constructing these process diagrams can increase the productivity of the business analyst and the architects involved in large projects.  <br> 
<br>
<br>
<br>
#### References
<br>
Most of the notations are taken from the modern definition of OMG BPM and OMG UML Activity Diagrams. <br>
<br>
Object Management Group  (OMG®)<br>
https://www.bpmn.org/ <br>
<br>
OMG® - Business Process Management Notation® (BPMN) - Definition <br>
http://www.omg.org/spec/BPMN/2.0/ <br>
<br>
OMG® - BPMN Version 2.0  <br>
https://www.omg.org/spec/BPMN/2.0/PDF <br>

* Section  11.7.2 Swimlanes (Page 363) <br>
* Section 10.2 Activities (Page 151) <br>
<br>
OMG® - Unified Modeling Language® (UML) Definition <br>
http://www.omg.org/spec/UML/  <br>
<br>
OMG® - UML Version 2.5.1  <br>
https://www.omg.org/spec/UML/2.5.1/PDF <br>

* Section 15. Activities  (Page 373) <br>
* Sub-section 15.5 Executable Nodes (Page 403) <br>
* Sub-section 15.6 Activity Groups (Page 405) <br>
<br>
<br>


## Swimlines
<br>

## Actors
<br>


## Activity 
All Activities should be named with the name of the operation performed (a verb) performed, and the entity (noun). <br>
The operation is a verb that in most cases can be one of the CRUD operations. For example: <br>

* "Create Invoice"
* "Read Invoice" (Search and Retrieve)
* "Update Invoice" ('Upsert' also permitted)
* "Delete Invoice"
<br>


## Top-to-bottom, Right-to-left 
<br>

## Process Start and End
Usually, Business Processes are documented as granular business interactions. sometimes it is better to break down a large process into several if the process is too big. <br>
Business Processes can be fitted at most in an A3 size page, but if the Activities are not readable, then it is a good decision to break it down into separate artefacts. <br>
So, the recommendation is that a Business Process must showcase clearly Actors performing business interactions. (In most cases these Actors will be performing business interactions with a system or platform). <br>
Each of the business interactions must be represented with a Start and a definitive End. However, this does not mean that in the same Business Process, there could be more than one business interaction. And each of them must have its own Start and End notation. 
<br>


## Conditions
<br>


## Sub-processes
<br>

## Applications
Generally, process diagrams include only one application where there is more than one actor, for example, a "User", or "Approver". However, there could be the case that the process describes a process that goes across applications or systems. The actors could be using more than one Application in the same process.
<br>

## Applications' components
Generally, the process diagrams describe an Application as a single participant or Actor in the process diagram. However, there could be the need to detail the Application in several components and describe some of the Application taxonomy. The Application will no longer be a single swimlane but two or more that will have different activities each. 
<br>
For example, an Application called "Zinga App", will have different components: 

* "Zinga App - Web". (the web frontend).
* "Zinga App - Backend". (and the server side).

In the case the application has a mobile version, this could be represented as <br>

* "Zinga App - Mobile". (for iOS and Android).
<br>
<br>
Breaking down the Application into more than one Entity could lead to adding unnecessary details to business processes. Process diagrams are not a substitute for Sequence Diagrams in terms of the amount of details that can be represented for describing system components' responsibilities.<br>
<br>
<br>
In addition, business processes don't need to represent any type of technology used or planned to be used. There are many cases business analysts add extra notations to signify what type of storage or database is used, or APIs, or Gateways, etc.  <br>
The only notation needed is the name of the operations (a verb) performed and the entity (noun). See the "Activity" section of this document.
<br>


## Colours
<br>

## Error Handling
Generally, business processes do not detail Error Handling, unless the error handling itself is a process that requires documentation because it consists of several steps that need to be coordinated across multiple Actors. Error Handling usually is considered a technical implementation and it is not part of the high-level process design. <br>
Business Processes only document happy paths and the most important permutations of the mainstream process.
<br>
<br>

## User Stories
<br>

## User Interface Screens
<br>

## Other References
Swimlane process - Wiki <br>
https://en.wikipedia.org/wiki/Swimlane <br>
<br>
Activity Diagram - Wiki <br>
https://en.wikipedia.org/wiki/Activity_diagram <br>
<br>
Swim Lane Diagram - CIO org <br>
https://cio-wiki.org/wiki/Swim_Lane_Diagram <br>
<br>
Flowchart - Wiki <br>
https://en.wikipedia.org/wiki/Flowchart <br>
<br>
ISO-5807 (1985)  <br>
https://www.scribd.com/document/519991367/ISO-5807-1985  <br>
https://www.iso.org/standard/11955.html
<br>
ISO-5807 (1985) PDF Document <br>
https://www.scribd.com/document/519991367/ISO-5807-1985  <br>
<br>
Flowcharting With the ANSI Standard paper 1971 - Old ISO and ANSI X3.5 standard flowchart symbols <br>
https://dl.acm.org/doi/pdf/10.1145/356566.356570 <br>
<br>
Business Process Modeling - Wiki  <br>
https://en.wikipedia.org/wiki/Business_process_modeling  <br>
<br>
Business Process Management (BPM) - Wiki <br>
https://en.wikipedia.org/wiki/Business_process_management <br>
<br>
Business Process - Wiki  <br>
https://en.wikipedia.org/wiki/Business_process  <br>
<br>
Process - Wiki   <br>
https://en.wikipedia.org/wiki/Process  <br>
<br>
Workflow - Wiki   <br>
https://en.wikipedia.org/wiki/Workflow   <br>
<br>
