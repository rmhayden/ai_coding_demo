I need an HTML/JavaScript code that will take a JSON, which the user should be able to copy and paste into an input in the web app, and then click a button such that 1) the JSON is converted into a CSV file and 2) the CSV file gets downloaded. The JSON is an array of objects, such that each object is a patient. All data should be included in the CSV output. The structure of the JSON for one patient object is shown below for reference. Please provide entire HTML/JavaScript code so that it can simply be copied and pasted.

patient = {
  "name": String,
  "age": Number, 
  "male": Boolean,
  "weightKg": Number,
  "sodiumValues": [
     {
       "sodiumValue": Number,
       "dateTimeStamp": String,
       “newTotalBodyWater”: Number,
       “predictedSodium”: Number
     }
   ],
   "waterGiven": [
     {
       "waterGivenCC": Number,
       "dateTimeStamp": String
     }
   ],
   “totalBodyWater”: Number,
   ”totalCations”: Number
}

