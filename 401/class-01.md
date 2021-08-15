# Read Class-01 :  Node Ecosystem, TDD, CI/CD
### Describe what **Array.map()** does :
The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.
* Parameters :
1. **element**
The current element being processed in the array.
2. **indexOptional**
The index of the current element being processed in the array.
* Return value
A new array with each element being the result of the callback function.
* Description
map calls a provided callbackFn function once for each element in an array, in order, and constructs a new array from the results. callbackFn is invoked only for indexes of the array which have assigned values (including undefined).

> It is not called for missing elements of the array; that is:
>1. indexes that have never been set;
>2. indexes which have been deleted.
### Describe what Array.reduce() does:
The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.
* Parameters :
1. **accumulator**
The accumulator accumulates callbackFn's return values. It is the accumulated value previously returned in the last invocation of the callback—or initialValue, if it was supplied2. **currentValue**
The current element being processed in the array.

* Return value
Your reducer function's returned value is assigned to the accumulator, whose value is remembered across each iteration throughout the array, and ultimately becomes the final, single resulting value.
* Description
The reduce() method executes the callbackFn once for each assigned value present in the array. 
>The first time the callback is called, accumulator and currentValue can be one of two values. If initialValue is provided in the call to reduce(), then accumulator will be equal to initialValue, and currentValue will be equal to the first value in the array. If no initialValue is provided, then accumulator will be equal to the first value in the array, and currentValue will be equal to the second.
### superagent();
`const superagent = require('superagent');`
`superagent.get('https://swapi.dev/api/people/')`
`.then(data =>{console.log(data.body)`
* **with Async/Await**
`async function cityFormat  (city) {`
`let result = await superagent.get('https://geocode.xyz/seattle?json=1');`
`console.log(result.body.longt,'---' ,result.body.latt)}`
### Explain promises as though you were mentoring a Code 301 level student:
JavaScript execute code lines line by line, and if there's a line code that takes time we give a "promise" so it won't wait for it to be finished and then go for the rest, javaScript will come back to that line at the time it being finished.
### Are all callback functions considered to be Asynchronous? Why or Why Not?
callback function doesn't make a function asynchronous.
Async callbacks are functions that are specified as arguments when calling a function which will start executing code in the background. When the background code finishes running, it calls the callback function to let you know the work is done, or to let you know that something of interest has happened.
