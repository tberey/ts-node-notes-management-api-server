# [ALPHA 0.0.1] Contact Lookup API (Node.js) - Early Build

***

## A RESTful Contact Lookup API, made in Node, that allows users to performs CRUD operations on a MongoDB Database.

### <i> At the moment this API is setup to allow the four basic crud operation for notes. I.e. {"title": "Test Title of Note", "body": "Test body of the note."} key-value pair, sent in the body of a POST/PUT request, to Create/Update a note in the DB, (in a x-www-form-urlencode). Notes are associated by ID for now.

***
***
|Version| Changes|
|:---|:---|
|Version 0.0.1 [2020-02-22]|<ul><li>Initial Commit.</li><li>Add "main.js" file, node project.</li><li>Add README.md</li><li>Make new dir "Screenshots".</li><li>Add some screenshots to "Screenshots" dir.</li></ul>|
|Version 0.0.2 [2020-02-22]|<ul><li>Split methods into routes, with a new "routes" dir, and a route script file for each CRUD Method. (Using modules/exports).</li><li>Add new DEL & GET methods to respective route script files.</li><li>Update POST method in POST script file, to add more data into the note records going into db.</li><li>Update README.md</li></ul>|