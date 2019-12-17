Sometimes you want to perform an action a number of times. 
For example : You want to print hello 3 times .
```js
	So you  will write : 
	
	1. console.log("hello")
	2. console.log("hello")
	3. console.log("hello")
	//hello
	//hello
	//hello
```
This is correct it is a  simple data  , we have to print it also 3 times only but what if there is a lot to print and the number of times to print also is huge like 50++ or 100++.

So here the `loops` are used .....

**Loops** 
help us to perform an action a number of times until a certain condition is met.


There are two types of loops  in js:

**Entry Controlled loops**

Here the   condition is tested before entering the loop body. ``For Loop`` and ``While Loop`` are entry controlled loops.

**Exit Controlled Loops**

Here the  condition is tested  at the end of loop body. Therefore, the loop body will execute at-least once, irrespective of whether the  condition is true or false. ``do – while loop`` is exit controlled loop.

![enter image description here](https://3.bp.blogspot.com/-7bYlZxBBB1U/WwRQN6cguJI/AAAAAAAAACA/BoA1fWJYTfEfnJ9rt4cZne4SBmR9l_OiACLcBGAs/s1600/slide_3.jpg)

Every loop contains 4 main things which are :

**Initialisation**

Here, we initialize the variable in use. It marks the start of a for loop. An already declared variable can be used or a variable can be declared, local to loop only.

**Condition**

It is used for testing the exit condition for a loop. It must return a boolean value. It is also an ``Entry Control Loop`` as the condition is checked before  the execution of the loop statements.

**Loop body**

The statements of what it should really do .

**Increment/ Decrement**

It is used for updating the variable for next iteration.



**while loop**


The condition occurs before  `statement` in the loop is executed. If the condition returns `true`, `statement` is executed and the `condition` is tested again. If the condition returns `false`, execution stops, and control is passed to the statement following `while`.

**Syntax**

```js
while  (condition )  {  
		//Statements to be executed repeatedly  
		// Increment (++) or Decrement (--) Operation  
	 }
```

**example**

```js

var i = 0
while ( i < 5 )  {
    console.log( i )
    i++;
	}
```
Here  `i` is a variable initialised and given the value as `zero` so as you know this is our starting point for the loop.Then there is a while condition where we are checking if our variable value is smaller than 5 , if true console the `i` , and then incrementing   the `i value`.



**for loops**

A  loop repeats until a specified condition evaluates to `false` .

**syntax**

```js

for ( initialisation ; condition ; increment;){
  //statement
  }
 ```
  **example**
  
  ``` js
  for (var x = 2 ;  x <=  4 ;  x++ )  {
		console.log();
	}
```
Here also same we are checking if the condition is true if true it will execute the statement and if false will come out of the loop block.

**for in**


The for in statement loops through the properties of an object.
The block of code inside the loop will be executed once for each property.

**syntax**

```js
for  (var  in  object) {  
	code block to be executed  
	}
```
**example**

```js
example 1:
var obj = {a: 1, b: 2, c: 3};
    
for (const prop in obj) {
  console.log(`obj.${prop} = ${obj[prop]}`);
}

// Output:
// "obj.a = 1"
// "obj.b = 2"
// "obj.c = 3"
```
```js
example 2:
const arr = [3, 5, 7];
for (let i in arr) {
   console.log(i); // logs "0", "1", "2", "foo"
}
```

**for of**


The for/of statement loops through the values of an iterable object.

**syntax**

```
for (variable of iterable) {
  statement
}  
```
**example**

```js
const iterable = [10, 20, 30];

for (const value of iterable) {
  console.log(value);
}
// 10
// 20
// 30
```


  **do while loop**
  
 
 do while loop is similar to while loop with only difference that it checks for condition after executing the statements, and therefore is an example of `Exit Control Loop.`

**Syntax**

```
do {
    statements..
}
while ( condition ) ;
```
**Example**

```
var x = 21;
do {
	console.log( x )
	x++;
}  while ( x < 20 ) ;
```
Here we execute  the statement and check the condition , if condition is true it will again iterate , if false it will come outside the loop.

