# Notes Lookup and Management API

## A locally hosted RESTful Notes Lookup API, made in TypeScript and Node with Express Framework, supported by a NoSQL MongoDB database. Allows users to performs CRUD operations on the database, using http requests.

### Create, search, update and delete personal notes/todos.

<br>

***

###### Client Page (Front-End) Homepage: <br>
#### <b>http://localhost:<Port\>/</b>

***

<br><i>

#### List of URL(http://localhost:<Port\>/) + URN (End-points), for Requests against a MongoDB, that are currently available:
| Endpoint | Method/Action on DB | Full URI (Using some port, e.g. "8080") |
|:---|:---|:---|
| <ul><li>"/"</li></ul> | <b><u>HOME/CLIENT PAGE</u></b> | <ul><li>"http://localhost:8080/"</li></ul> |
| <ul><li>"/new"</li></ul> | <b><u>POST/Create</u></b> | <ul><li>"http://localhost:8080/new"</li></ul> |
| <ul><li>"/all"</li><li>"/<noteID\>"</li></ul> | <b><u>GET/Read</u></b> | <ul><li>"http://localhost:8080/all"</li><li>"http://localhost:8080/<noteID\>"</li></ul> |
| <ul><li>"/<noteID\>"</li></ul> | <b><u>PUT/Update</u></b> | <ul><li>"http://localhost:8080/<noteID\>"</li></ul> |
| <ul><li>"/<noteID\>"</li><li>"/deleteAll"</li></ul> | <b><u>DEL/Delete</u></b> | <ul><li>"http://localhost:8080/<noteID\>"</li><li>"http://localhost:8080/deleteAll"</li></ul> |


***

***

<br>

|Version| Changes|
|:---|:---|
|Version 0.0.1 [2020-02-22]|<ul><li>Initial Commit.</li><li>Add "main.js" file, node project.</li><li>Add README.md</li><li>Make new dir "Screenshots".</li><li>Add some screenshots to "Screenshots" dir.</li></ul>|
|Version 0.0.2 [2020-02-22]|<ul><li>Split methods into routes, with a new "routes" dir, and a route script file for each CRUD Method. (Using modules/exports).</li><li>Add new DEL & GET methods to respective route script files.</li><li>Update POST method in POST script file, to add more data into the note records going into db.</li><li>Update README.md</li></ul>|
|Version 0.1.0 [2020-02-23]|<ul><li>Add a whole set of CRUD operation on db, using GET http Requests.</li><li>Add error handling for each route file's request. As in all requests will check to see it is a valid action.</li><li>Create/Update notes with omitted query strings won't be nullified.</li><li>General improvements/bug fixes.</li><li>Comments tidy-up & testing.</li><li>Update README.md</li></ul>|
|Version 0.1.1 [2020-02-24]|<ul><li>Began work on front-end back-end connection, with a temporary setup (using get rquests & query string, in a iframe - for now).</li><li>Add "index.html", which will serve as front end.</li><li>Tested object transfer from middle-ware to back end, to begin work on new methods for front end.</li><li>Add mp4 video demo to screenshots dir.</li><li>Update README.md</li></ul>|
|Version 0.2.0 [2020-02-25]|<ul><li>Major Front-End Update</li><li>Serve "index.html" client landing page</li><li>Connect front with back, via AJAX in the front end.</li><li>Add new screenshot and rename most. Also remove old screenshot.</li><li>Update README.md</li></ul>|
|Version 0.2.1 [2020-02-26]|<ul><li>Replace GET method for adding a new note to a POST, in "index.html".</li><li>Add Delete All (DELETE Request) to front end.</li><li>Update server POST Method in routes, to receive parameters from client.</li><li>Update README.md</li></ul>|
|Version 0.2.2 [2020-02-27]|<ul><li>Add front-end request methods: Update (PUT), Delete (DELETE) & Search (GET), via buttons/input fields.</li><li>Add new sub-input area, with new field and new button (html/css).</li><li>Update README.md</li></ul>|
|Version 0.2.3 [2020-02-28]|<ul><li>Fix front-end bug, where updated note showing as undefined on page.</li><li>Add new key value pair to note (note number), also displayed to html.</li><li>Update README.md</li></ul>|
|Version 1.0.0 [2020-02-29]|<ul><li>1.0.0 Release!</li><li>Complete front-end: finalise all ajax requests performed.</li><li>Adjust search via new sorted, better ID number system</li><li>Complete all error handling, including console errors, for all requests/methods.</li><li>Update Screenshot rep, all contents</li><li>Split "index.html" scripting into it's own new dir: scripts/ with filename: "requests.js", as it performs at ajax requests for index page, via JS.</li><li>Update README.md</li></ul>|
|Version 1.1.0 [2020-03-27]|<ul><li>TypeScript Update</li><li>Upgrade project to TypeScript (back-end).</li><li>Various code additions, adjustments, new dependancy modules or imports/exports, to accomodate the TypeScript upgrade.</li><li>Update README.md</li></ul>|
|Version 1.1.1 [2020-03-30]|<ul><li>Finish setting types, and defining exported/imported interfaces.</li><li>Add error-handling/catch all; any user attempting to visit/GET any incorrect URI is redirected to the notes index client page.</li><li>Update README.md</li></ul>|
|Version 1.1.2 [2020-04-02]|<ul><li>Update and correct all types for routing.</li><li>Update README.md</li></ul>|
|Version 1.1.3 [2020-05-22]|<ul><li>Update namings and descriptions.</li><li>Update README.md</li></ul>|
|Version 2.0.0 [2020-06-01]|<ul><li>TypeScript & Class Update - Whilst already a TypeScript project, it has been further updated to make more and better use of TypeScript features, as well as reconstructed into a more object oriented and class based design. Also sharpened up the code, fixing any mistakes, inconsistencies, or general improvements.</li><li>EJS Update - Whilst already a EJS Templated project, it has been further updated to make more and better use of ejs engine features, as well as compacting the code, fixing any mistakes/bugs, inconsistencies, and general improvements.</li><li>More to come... to finish ejs/client-scripting side of things.</li><li>Update README.md</li></ul>|