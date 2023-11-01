# Promises in Javascript 

 Javascript is asynchronous by its nature , so the code in the application might be executed in another order than its written . Promises can be used to handle this  kind of situations.

 ## why we need Promises 

   In our application if we have a three blocks of  code written in their correct flow of execution , we cant garuntee that the code will run successfully even though our code is correct. Because if we have a http request in our second block of our code , usually http requests takes more time to process and get the data , but the javascript code will start executing the code in block 3 also which is dependent on the results of code in the block 2 . In this way our code fails successful execution because the 3rd block is executed without getting all the necessary data from the block 2 .

   ## What is a Promise 

   A Special object that represents  a eventual completion of an asynchronous operation.

   Every promise object have two properties .

   1. Status -  It can contain 1. pending 2. fulfilled 3. rejected 

 2. Value  - It can contain any js value , even undefined 

 This type of asynchronous execution can be handled in two ways 
 1. Pass a Callback

 2. Return a Promise 
 

 ## Status of the Promise

 ---

 The Status of a promise can be Pending , Fullfilled ( Resolved )
 or Rejected .


  ### Syntax
  const promise1 = new Promise( function(resolve , reject){resolve("Hello World")})

 Here the promise status is resolve and the value is "Hello World"

  * Once a promise is made as resolved , we cant update  or change its status to rejected and  Vice Versa 


 ### Promise Methods 

 * Then() method
 
 1. 1st one is the function to be executed when the promise is resolved and this function takes the value of the promise as a parameter

 2. 2nd one is the function to be executed when the promise is rejected and this function takes the reason (The reason for the failure of the promise) as a parameter .

### Chaining Promises 

 - Then method takes two arguments and returns a promise object.
 
  - Therefore we can invoke another then method as the return of the previous then method 
  This is called  Promise Chaining 

  Note :  For the promise which we are used in the return of first promise also we need to give the two arguments (resolve and reject).
  