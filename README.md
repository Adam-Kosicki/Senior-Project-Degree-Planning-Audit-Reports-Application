# Senior-Project---Degree-Planning-Audit-Reports

Degree Audit Program
Table of Contents
I. Project Metrics
II. Implementation Details
III. Impact and Security
IV. Individual Assessment
V. Issues and Lessons Learned
VI. Future Work
VII. Appendix
VIII. Timetable

I. Project Metrics
This semester, our team successfully created a large part of the Degree Audit Program. Despite not delivering every feature, we utilized our combined knowledge to develop a program we are proud of. Working on a complex system from scratch presented challenges we hadn't faced before, but it provided valuable experience in teamwork towards a common goal.

As a team, we achieved the following:

Implemented several GUI panes
Enabled transcript selection and parsing
Implemented data storage using a Student object
Provided editable options for the audit
Implemented printing and saving of the degree audit
Generated the majority of the Degree Plan
II. Implementation Details
Our team used the IntelliJ IDE to code the project, employing Java APIs such as PDFBox for parsing and Java Swing for the GUI components. The project consists of eight classes:

DegreePlanApp - The main class in charge of initializing the GUI and prompting the user to select a file. It calls the PDFParser class to tokenize the transcript data and returns it as a Student object. It then creates a degree audit and calls GenerateEditableDegree to create the degree plan.
StartUp - Creates the first GUI window for the user to select a Transcript or a Student file using a file selector from JSwing.
PDFParser - Extracts data from the PDF Transcript selected by the user, such as name, ID, and courses.
Student - Stores data for each student, including name, ID, courses, prerequisites, enrollment date, and more.
Course - Keeps track of available courses and formats them as an array of Course objects.
GenerateEditableDegree - Passes Student information to SpreadsheetUI for degree plan generation.
SpreadsheetUI - Generates the editable degree plan using a spreadsheet UI through APIs.
StudentSave - Saves the Student object as its own file type for later retrieval.
III. Impact and Security
Impact:

Improved Student Experience: The program offers a user-friendly platform for students to navigate, plan, and edit their degree courses, visualizing their academic progress and enabling informed decisions about future course selection.
Improved Student Retention: The tool assists students in tracking their academic progress, leading to improved retention rates.
Increased Efficiency: Advisors can access a student’s degree plan quickly, providing targeted guidance and support, thus streamlining academic planning.
Security:
The project is yet to integrate security measures. However, we acknowledge the importance of safeguarding sensitive information. Implementing robust security features such as password protection, data encryption, and access control will ensure confidentiality and integrity of user data, building trust with users and stakeholders.

How to Run the Program:

Ensure JDK 19 is installed.
Download and extract the Cap_Proj zip folder.
Navigate to 'Cap_Proj -> out -> artifacts -> Cap_Proj.jar'.
Run the Cap_Project executable jar file to begin.
IV. Individual Assessment
Our team members played essential roles in various aspects of the project:

Adam Kosicki (Project Lead): Initiated the project, managed deadlines, implemented saving/loading of student objects, and provided technical contributions to the GUI.
Adrian Sanchez (Transcript and Audit): Responsible for reading transcripts, tokenizing data, and generating the audit report. Worked on printing various audit components.
Jonathan Vu (DegreePlan): Developed the DegreePlan component, generating degree plans from user data and transcripts.
Grant Reed (Application Start and Options): Managed application startup, wrote code for options fields, and assisted with team coordination and motivation.
Jason Vu (Student Class and GUI): Developed the Student class, improved serialization, and designed the GUI for displaying degree plans.
Michael Wu (Degree Plan GUI): Implemented GUI for the degree plan, allowing for edits and saving/printing the plan.
V. Issues and Lessons Learned
We have compiled step-by-step instructions in the appendix for installation, usage, and extension of the program. We also learned valuable concepts from previous courses, like regular expressions and Maven for build automation.

To improve the senior design course, we recommend incorporating more real-world, industry-oriented projects and providing explicit guidance on using tools like Maven and GUI frameworks. Encouraging teamwork and interdisciplinary projects can enhance students' preparation for professional software development.

VI. Future Work
Given more time, we suggest implementing error handling, validation checks, and machine learning algorithms to enhance accuracy. We would also improve the user interface, adding interactive features and integrating other educational resources.

VII. Appendix
We have included a list of useful references that guided us during development, including official documentation for Apache PDFBox, Java Regex, Apache POI, Maven, and Java Swing.

VIII. Timetable
Outlined the project's phases, from reading PDFs and extracting information to generating the audit report and implementing the GUI.
