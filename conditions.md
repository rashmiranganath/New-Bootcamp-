 
Decision making 

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

```html
if (condition) {
  // block of code to be executed if the condition is true
}
```

**example**

```html
if (10 > 5) {
    console.log("this is a if statement");
}
```
As we came to know if statements get executed if the given condition is true so in this example the condition is (10>5) ,and  10 is always greater than 5 so the condition is true , statements inside this block will get executed.

**else condition**

The if statement specifies a block of code to be executed if a condition is false.

**syntax**
```html
if (condition){ 
code to be executed if condition is true
}

else {
code to be executed if condition is false
}
```

**example**
```html
if (10 < 5) {
    console.log("this is a if statement");
}
else{
  console.log("this is a false statement")
}
```
Here we are checking the if statement first (10 < 5) the condition is false because 5 can never be greater  than 10 , so here the else statement performs its role and executes the else block.

**Else if**

This statement is used when your first condition is false but still you want to check it by other conditions .It can have multiple else if conditions if you want to check multiple conditions. 

**syntax**

```html
if (condition){
  code will be executed if condition is true
}
else if(condition) {
  code will be executed  if the following condition is true
}

else{
  this will be executed if both the if and else if conditions are false
}
```

**example**
```html
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

```switch (expression)
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
    .
    case valueN:
        statementN;
        break;
    default:
        statementDefault;
}
```

1 .An expression that needs to be checked – In this statement, we check the expresAn expression that needs to be checked – In this statement, we check the expression which needs to be evaluated. Based on the execution of expression the switch case satisfying will be executed.

2.Different cases – On the execution of an expression, the case which satisfies the expression gets executed.

3.Default case – If any of the switch cases do not get satisfied then the default case is executedsion which needs to be evaluated. Based on the execution of expression the switch case satisfying will be executed.


**example**
```
let a = 2 + 2;

switch (a) {
  case 3:
    console.log( 'Too small' );
    break;
  case 4:
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
