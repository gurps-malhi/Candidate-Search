html created an id tbData, this is where i will create the table of candidates using javascript.

html id of txtTerm will be used to get the value of the search query, the click event will call the SearchTerm() function.

javascript:

Empty Array created
created an empty object called allPersons - this will hold the details of the candidates

person object created 
properties of:identifier, first, last, age, email, profile.  

function InsertPersonToTable 
-Function used to create the table is InsertPersonToTable with parameters of the table id and the new instance of the person object
-Created a div element named and defined it within var rowDiv, gave it a class name of "row"
-used concatenation to build the table of contact with span classes and the properties of the person object 
-table(rowDiv) appended to tbData.
-the empty array is populated with the details of the person object 

function ShowProfileDetails(id)
-removes the summary details of candidates
-calls the GetPersonDetailsAsHTMl(id) function which builds the more details table this also has the back button click event  


function BackToList()
-display blocks the tbData div
-displays none the dvMoreDetails (more candidate details)

function UpdateTableForSearch(arrResults)
Creates a new table based on the search results calls InsertPersonToTAble function 

function searchterm
actually does the search if matches search criteria, run above function else output failure message

How it works:

Every time you wish to create a new candidates just create a new instance of the person object with the relevant properties for profile you can add a string to a variable and use that in the object instance.