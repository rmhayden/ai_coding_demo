I want a simple JavaScript and HTML code (all in one HTML script so I can simply copy/paste the whole script for one file) that will show on the web browser page the value for each object in an array, where the object has the following structure: 

const patients = [ 
{ 
"name": String, 
"age": Number, 
"male": Boolean, 
"weightKg": Number, 
"sodiumValues": [ 
{ 
"sodiumValue": Number, 
"dateTimeStamp": String 
} 
], 
"waterGiven": [ 
{ 
"waterGivenCC": Number, 
"dateTimeStamp": String 
} 
] 
} 
] 

The input JSON should go into an input field, such that the user can copy/paste the input JSON before clicking a button that renders it within the application.

