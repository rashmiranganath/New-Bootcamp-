**Arrays**

In JavaScript, an array is a variable that is used to store different data types which means it basically stores different elements in one box and can be later accessed with the variable.

**syntax**
There are two ways to declare an array:
```js
Method 1

var array = [ ele-1 , ele-2 , ...., ele-n]

Here we are declaring the array by using square brackets 



Method 2

var array = new Array(ele-1 , ele-2 ,.... ele-n]

Here we are using new Array keyword to declare it.

```

**Accessing Array Elements**
Elements of the array can be accessed through their indices or index.The index of the array starts from 0 to n number of elements.
 example :
 ```js
 var array1 = ["apple", "banana", "orange"]
 ```
 Here i can access the first element of the array by using the array name and its index which is : `array1[0]`

**Length of the array**
We can get  an array's length by using the length function.
example:
```js
var  collection = ["rashmi", "komal", "kiran" , "Mohan"]
``` 
`collection.length` will give me the array length.
Array length will always start from 1.If the array is empty then the length is 0.


![enter image description here](https://www.sitesbay.com/cpp/images/cpp-array.png)



**Why Arrays???**
1. Array is an object which stores collection of different data type elements orderly.

2. Helps us to access a particular element in the array.

3. Can access the elements one by one using a loop.
```javascript
			index = 0
			array = [ 1, 2, 3, 4, 5, 6 ]
            while(index < array.length) {
		        console.log(array[index])
		        index++
			 }  
Answer -
//1 , 2 , ............ 6 

It will console all the elements in the array one by one accordingly
 with the help of loop.
```


4. **Methods** are used in array to perform different functionalities on the array according to the user's choice.

example : push() , pop() , shift() , unshift()

There are multiple methods available which can be used according to our requirement.Few frequently used methods are as follows:

**-push()**
This method adds items to the end of an array and  `changes`  the original array.
```javascript
let browsers = ['chrome', 'firefox', 'edge'];
browsers.push('safari', 'opera mini');
console.log(browsers); 
// ["chrome", "firefox", "edge", "safari", "opera mini"]

```


**-pop()**
This method removes the last item of an array and  `returns`  it.

```javascript
let browsers = ['chrome', 'firefox', 'edge'];
browsers.pop(); // "edge"
console.log(browsers); // ["chrome", "firefox"]
```

**-shift()**
This method removes the first item of an array and  `returns` it.

```javascript
let browsers = ['chrome', 'firefox', 'edge'];
browsers.shift(); // "chrome"
console.log(browsers); // ["firefox", "edge"]
```

**-unshift()**

This method adds an item(s) to the beginning of an array and  ****changes****  the original array.

```javascript
let browsers = ['chrome', 'firefox', 'edge'];
browsers.unshift('safari');
console.log(browsers); //  ["safari", "chrome", "firefox", "edge"]
```

**-splice()**

This  method  `changes`  an array, by adding, removing and inserting elements.

The syntax is:

```
array.splice(index[, deleteCount, element1, ..., elementN])
```

-   `Index`  here is the starting point for removing elements in the array
-   `deleteCount` is the number of elements to be deleted from that index
-   `element1, …, elementN` is the element(s) to be added

```javascript
let colors = ['green', 'yellow', 'blue', 'purple'];
colors.splice(0, 3);
console.log(colors); // ["purple"]
// deletes ["green", "yellow", "blue"]
```

If the second parameter is not declared, every element starting from the given index will be removed from the array:

```javascript
let colors = ['green', 'yellow', 'blue', 'purple'];
colors.splice(3);
console.log(colors); // ["green", "yellow", "blue"]
// deletes ['purple']
```
In the next example we will remove 3 elements from the array and replace them with more items:

```javascript
let schedule = ['I', 'have', 'a', 'meeting', 'tommorrow'];
// removes 4 first elements and replace them with another
schedule.splice(0, 4, 'we', 'are', 'going', 'to', 'swim');
console.log(schedule); 
// ["we", "are", "going", "to", "swim", "tommorrow"]
```

**-indexOf()**

This method looks for an item in an array and returns  'the index'  where it was found else it returns  `-1`

```javascript
let fruits = ['apple', 'orange', false, 3]
fruits.indexOf('orange'); // returns 1
fruits.indexOf(3); // returns 3
friuts.indexOf(null); // returns -1 (not found)
```

**A list of methods which you can use **
-   ****toString()**** converts an array to a string separated by a comma.
-   ****join()**** combines all array elements into a string.
-   ****concat****  combines two arrays together or add more items to an array and then return a new array.
-   ****push()****  adds item(s) to the end of an array and  ****changes****  the original array.
-   ****pop()****  removes the last item of an array and  ****returns****  it
-   ****shift()****  removes the first item of an array and  ****returns****  it
-   ****unshift()****  adds an item(s) to the beginning of an array and  ****changes****  the original array.
-   ****splice()****  ****changes****  an array, by adding, removing and inserting elements.
-   ****slice()****  copies  a given part of an array and returns that copied part as a new array.  ****It does not change the original array.****
-   ****split()****  divides a string into substrings and returns them as an array.
-   ****indexOf()****  looks for an item in an array and returns  ****the index****  where it was found else it returns  `-1`
-   ****lastIndexOf()****  looks for an item from right to left and returns the last index where the item was found.
-   ****filter()****  creates a new array if the items of an array pass a certain condition.
-   ****map()****  creates a new array by manipulating the values in an array.
-   ****reduce()****  calculates a single value based on an array.
-   ****forEach()****  iterates through an array, it applies a function on all items in an array
-   ****every()****  checks if all items in an array pass the specified condition and return true if passed, else false.
-   ****some()**** checks if an item (one or more) in an array pass the specified condition and return true if passed, else false.
-   ****includes()****  checks if an array contains a certain item.


**Questions**
1. Find the 2nd max number in the given array.
	var a = [ 7 ,9 ,34 ,678 , 1, 67 ,43 ]

2. Remove the duplicates from the given array.
var array = [ [10 , 6 ,5 ,7] , [ 6 ,42 , 7 , 0 ] ,[ 1 ,7, 98 , 5 , 42] ]


