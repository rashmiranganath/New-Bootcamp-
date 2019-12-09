**Decision making**

Making,`decisions` in programming is similar to decision making in real life. In programming also we face some situations where we want a certain block of code to be executed when some `condition is fulfilled`.

This is where `Conditionals statements` come into place

**Conditional Statements**
Conditional statements are used to decide the flow of execution based on different conditions. If a condition is true, you can perform one action and if the condition is false, you can perform another action.

  ![condition](https://www.guru99.com/images/JavaScript/javascript5_1.png)

 **There are four types of conditional statements :**
 
1. if statement
2. else statement
3. else if statement
4. switch case

  
**if statements**
The if statement specifies a block of code to be executed if a condition is true.

**syntax**
```
if (condition) {
// block of code to be executed if the condition is true
}
```
**example**
```
if (10 > 5) {
console.log("this is a if statement");
}
```
As we came to know if statements get executed if the given condition is true so in this example the condition is (10>5) ,and 10 is always greater than 5 so the condition is true , statements inside this block will get executed.

 **else condition**
The if statement specifies a block of code to be executed if a condition is false.

 **syntax**
```
if (condition){
code to be executed if condition is true
}
else {
code to be executed if condition is false
}
```
**example**
```
if (10 < 5)  {
console.log("this is a if statement");
}
else {
console.log("this is a false statement")
}
```
Here we are checking the if statement first (10 < 5) the condition is false because 5 can never be greater than 10 , so here the else statement performs its role and executes the else block.

  **Else if**
This statement is used when your first condition is false but still you want to check it by other 
conditions .It can have multiple else if conditions if you want to check multiple conditions.

**syntax**
```
if (condition){
code will be executed if condition is true
}
else if(condition) {
code will be executed if the following condition is true
}
else{
this will be executed if both the if and else if conditions are false
}
```
**example**
```
if (10 < 5 ) {
console.log("this is a if statement" )
}
else if (5==5) {
console.log("this is a else if statement" )
}
else {
console.log("this is a false statement" )
}
```
Here we are checking the if statement which is false but we want to check another condition instead of taking the else value , so here to increase our conditions we are using else if so that even if condition is false we can check one more condition and then if that also false it will landup in the else condition.

Note: A program can have multiple `if` and `else if` conditions but only one `else` condition.

**Switch case**
Switch case is also a decision making mechanism like if-else conditions in js.
Its syntax is more simple .

**syntax**
```
switch (expression)
{
case value1:
		statement1;
		break;
case value2:
		statement2;
		break;
.
.
.
case valueN:
		statementN;
		break;

default:
		statementDefault;
		}
```
1 .An expression that needs to be checked – In this statement, we check the expression expression that needs to be checked – In this statement, we check the expression which needs to be evaluated. Based on the execution of expression the switch case satisfying will be executed.

2.Different cases – On the execution of an expression, the case which satisfies the expression gets executed.

3.Default case – If any of the switch cases do not get satisfied then the default case is execution which needs to be evaluated. Based on the execution of expression the switch case satisfying will be executed.

  **example**

```
let a = 2 + 2;
switch (a) {
case 1:
	console.log( 'Too small' );
	break;
case 2:
	console.log( 'Exactly!' );
	break;
case 5:
	console.log( 'Too large' );
	break;
default:
	console.log( "I don't know such values" );
}
```
In this code variable `a` stores the `value of 4 `,and we are checking which value will be equal to this variable . In switch case as you all know we check the `conditions through cases` . If any `case is equal to the variable value` it will go inside that case and execute the code in that block , or if the `cases is false` then it will move to the other cases.If `all the cases are false` by default it will execute the default statement only if `mentioned`.

  
  

**Ternary operator**
The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is true followed by a colon (:), and finally the expression to execute if the condition is false. This operator is frequently used as a shortcut for the if statement.

**syntax**
```
condition  ?  value if true : value if false
```
1.  The  `condition`  is what you’re actually testing. The result of your condition should be  `true`  or  `false`  or at least coerce to either boolean value.
2.  A  `?`  separates our conditional from our  `true`  value. Anything between the  `?`  and the  `:`  is what is executed if the  `condition`  evaluates   `true`.
3.  Finally a  `:`  colon. If your  `condition`  evaluates to  `false`, any code after the colon is executed.

**example 1**
```
var ans = if (4-2 = 2) ? true : false;
console.log(ans)
```
Here is a simple ternary operator code where we have given a condition and  the condition is full-filled the first statement will execute . If false then the next statement will execute.

**example 2**
```
let isStudent = true;
let price = isStudent ? 8 : 12
console.log(price);  
// 8
```
Here in this code i have initialized a variable as true  by default .
In the condition below i have given that variable only as condition . As you know by default the value is true so it will execute the 1st statement only which is 8.

**Questions**

question 1 -
``` 
if ( "a" == "a"){
	console.log("yippee you win")
}
console.log("you loose")
```
Answer -

// yippee you win

// you loose 

`Here we have a condition which is true so the statement in the if block will be executed.
Later it comes out of the if block  and executes the next line which says console.log("you loose") , because we have not mentioned any else statement its just a normal next line code after the if statement.																			 

Note : If this program had a else statement or else if they both would never be executed because the first statement is true after that it would break the flow of other conditions below.`

question 2-
```
var a = 10
 
if (a == 10) {
console.log(a)
	if( a % 2 == 0){
	console.log("divisible by 2")
	}
	else {
	console.log("not a divisible of 2")
	}
}
else {
console.log("wrong answer")
}
```
Answer - 

//10

//divisible by 2


Here in this code there is a if statement inside an if statement , these are called as nested if else statements. So it works as follows if the first condition is full-filled then it will go inside the if block , there also we have given an nested if statement so it will check its condition if full-filled it will execute its statement, if not full-filled it will go to the nested else statement and execute the statement.
If the nested if is not full filled it will execute the else condition in this code .

question 3-
```
var day = 10;
var text = " "
switch (day) {  //day is an integer varying from 0 to 6.
    case 6:
        text = "Today is Saturday";
        break;
    case 0:
        text = "Today is Sunday";
        break;
    default:
       text = "Looking forward to the Weekend";
} 
console.log(text)
```

Answer-

//Looking forward to the Weekend 


Here is a switch case with 3 different cases , the switch case as you know acts like if else statement only , in this code both the cases are not full-filled so it takes default case and executes the statement in the default block and ends the program.

question 4-
```
let isStudent = false;  
let isSenior = true;
let price = isStudent ? 8 : isSenior ? 6 : 10
console.log(price);  
```
Answer - 

// 6

We can nest ternary operators to test multiple conditions.
Here we are testing two conditions , the first condition is false so the statement which is false expression will get executed, which is `isSenior`  and here its nested ternary operator .The `isSenior' becomes another condition and its value is true so it returns the true statement which is 6.




