# Sprint 03 Reflection
UNA CSIS CAPSTONE
JOBIE SCRUM TEAM DELTA 


Task: Clean up uploads
Problem: Multiple pages link to the same database and pulled into upload file

Requirements:
A JOBIE user with an established account & logged into the system. Web browser. Access to http://buildingthepride.com/jobie/uploads/ and JOBIE database and pull files.

Design: <a href = "Sprint3Reflection/WEB_URLinfo.docx " target="_blank">web_info</a>

`Add or edit page for users to see review status of a submission
viewPublication.php

page initialized with sesion_start, header.php, sidebarmenu.php, dbConnect.php, viewPublicationContent.php
page ends with footer.php
viewPublicationContent.php

initialize session, gets user ID and Role
One major Function: viewPublication();
Allows a user with the 3003 role(admin) to make changes to the selected publication's info
If changes are made, INSERT into following tables ..* volume ..* year ..* season
If unable to connect to DB, sends error back.
spring2011.php(and other spring.php files)

Initializes with session_start()
requires header.php and sidebar.php
Each file has only one function: spring20XX(); (replace XX with the year of the file)
Function calls to the database and displays all articles for the year's publication, and provides a download link
TODO: Change download button to preview, and get all files turned into .pdf's in the database.
