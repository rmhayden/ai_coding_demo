I need a script (one single file with JavaScript and HTML that will display in a web browser) that will take a JSON (that can be copied and pasted into an input on the web browser) and perform a series of functions outlined in the below instructions to create a new modified JSON, which will show up in the web browser as well. Below is the structure of the original JSON:

patient = {
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

The format of the dateTimeStamp string, which provides the date/time stamp, is like this example: "2026-02-02T06:00"

There should be a download button that allows the user to download the new modified JSON file.

Here are the instructions to take the initial JSON and end up with the new modified JSON:

For each patient, add a key-value pair for “totalBodyWater” (weight x 0.5)

For each patient, add a key-value pair for “totalCations”, which is equal to totalBodyWater x the value of the first sodiumValue within sodiumValues

For each patient’s sodiumValues objects (except for the first in array, which will have a value of ”null” for each new variable), do the following:

Add a key-value pair to the sodiumValues object for “newTotalBodyWater”, which is equal to the original value of patient’s total body water plus any additional “waterGivenCC” up until the point in time for the dateTimeStamp value of that sodiumValue

Add a key-value pair to the sodiumValues object for “predictedSodium”, which is equal to “totalCations” for the patient divided by “newTotalBodyWater” for that given sodiumValues object, as already calculated in prior step


