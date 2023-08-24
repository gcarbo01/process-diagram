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
In large programs, the business process is the best artefact that can be used to describe the functionality, scope, actors and functional permutations. Business Processes, if used correctly, can include a large number of Actors, multiple Applications, online and offline activities, can indicate sequentially, can break down large processes into sub-processes, and other benefits. And others.<br> 
After these processes are finalised, they are usually used as input for many other consequent works, including Architects, who receive them and consider them as input for business requirements and system requirements. <br> 
Sometimes, Architects need help reading these business processes because they are not detailed enough, or the notations and standards used to document them make them ambiguous. So, to streamline the work of business analysts and architects, it is better to adopt some standards and notations beforehand. This way, the documented business processes can be transformed into functional and system requirements. So, the Architects need to collaborate with the Business analysts to understand these diagrams and transform them into business and system requirements. <br> 
If there are no standards or agreements on the use of notations, then the business processes are created with different styles, and usually, there is also a difference in the documentation if more than one business analyst works on them.  Sometimes, business analysts have different skills and opinions on how much detail these diagrams should have, and if there is no guidance, they use their criteria.  Some business analysts may use a high-level approach to describe the business flows. On other occasions, they may use detailed notations to describe business logic. <br> 
This article proposes guidance and the adoption of specific notations; it discusses the benefits and other options for some scenarios when documenting large business processes. The guidance is based on the standards proposed by BPMN and UML, particularly the swimlane process diagrams and the activity diagrams intersection. <be>
With this guidance, business analysts can collaborate seamlessly. The architects can now use the business processes as they have been produced as input for their solutions, architecture design, and applications. <be>
Also, the product owners or scrum masters can benefit from these guidances because they can use these business processes as input for their agile process, in particular, to define epics and create user stories.  <br> 
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
<br>

<img src="./images/BPMN-sample1.jpg" align="center" width=75% height=75%>

## Swimlines
<br>
<br>
<br>

## Actors
<br>
<br>
<br>


## Activity 
Activities signify a granular task that are performed. It is important to notice that there could be off-line Activities and on-line Activities, which are meant to be part of an application, system or platform. <be>
Off-line Activities can be named as best described, for example, by using a verb and nouns: "Collect a pamphlet", "Ring the bell". <br>
On the contrary, Online-Activities' names can be more structured since they are meant to be digitised; therefore, they should be named as the operation performed (a verb) and the entity (noun). <br>
The operation is a verb that, in most cases, can be one of the CRUD operations. For example: <br>

* "Create Invoice"
* "Read Invoice" (Search and Retrieve)
* "Update Invoice" ('Upsert' also permitted)
* "Delete Invoice"

<br>
<br>
<br>

## Top-to-bottom, Right-to-left 
<br>
<br>
<be>

## Process Start and End
### Business Interactions
Usually, Business Processes are documented as granular business interactions. Sometimes, it is better to break down a large process into several if it is too big. <br>
Business Processes can be fitted at most in an A3 size page, but if the Activities are not readable, it is a good decision to break it down into separate artefacts. <br>
So, the recommendation is that a Business Process must showcase Actors performing business interactions. (Usually, these Actors will perform business interactions with a system or platform). <br>
Each business interaction must be represented with a Start and a definitive End. However, this does not mean there could be more than one business interaction in the same Business Process. And each of them must have its own Start and End notation. 
<br>
### Temporal Events
<br>


## Conditions
<br>


## Sub-processes
<br>

## Applications
Generally, process diagrams include only one application with more than one actor, for example, a "User" or "Approver". However, the process describes a process that goes across applications or systems. The actors could be using more than one Application in the same process.
<br>

## Applications' components
Generally, the process diagrams describe an Application as a single participant or Actor in the process diagram. However, there could be the need to detail the Application in several components and describe some of the Application taxonomy. The Application will no longer be a single swimlane but two or more with different activities each. 
<br>
For example, an Application called "Zinga App", will have different components: 

* "Zinga App - Web". (the web frontend).
* "Zinga App - Backend". (and the server side).

In the case the application has a mobile version, this could be represented as <br>

* "Zinga App - Mobile". (for iOS and Android).
<br>
<br>
Breaking down the Application into multiple sub-components could add unnecessary details to business processes. Process diagrams are not a substitute for Sequence Diagrams in terms of the amount of details that can be represented for describing system components' responsibilities.<br>
<br>
<br>
In addition, business processes can be used without representing any technology used or planned to be used. There are many cases in which business analysts add extra notations to signify what type of storage or database is used, or APIs, or Gateways, etc.  <br>
The only notation needed is the name of the operations (a verb) performed and the entity (noun). See the "Activity" section of this document.
<br>


## Colours
<br>

## Error Handling
Generally, business processes only detail Error Handling if the error handling itself is a process that requires documentation because it consists of several steps that need to be coordinated across multiple Actors. Error Handling is usually considered a technical implementation and is not part of the high-level process design. <br>
Business Processes only document happy paths and the most important permutations of the mainstream process.
<br>
<br>
<br>

## User Stories
<br>
<br>
<br>

## User Interface Screens
<br>
<br>
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
<br>
<br>>
