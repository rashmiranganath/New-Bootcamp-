
**Objects**
- Store data in form of key and values.
- Object is a non-primitive data type in JavaScript.
- An object holds multiple values in terms of properties and methods.
- Properties can hold values of primitive data types.
- Functions in objects are known as methods.
```
var car = {
	name  : "xyz",
	brand : "abc",
	price : 2345
}
```
Here is an example for an object , it has keys like name , brand , price and those keys have a corresponding values also like xyz , abc , 2345 . This is only an example of a object's structure.
	

**Why most of the things in js are  object ?**

```js
var store = {};
store.test = 'foo';
store.test; // 'foo' (therefore, object) 

var jobs = [];
jobs.test = 'foo';
jobs.test; // 'foo' (therefore, object)

var log = function() {};
log.test = 'foo';
log.test; // 'foo' (therefore, object)

var total = 1;
total.test = 'foo';
total.test; // undefined (therefore, not object)

var greeting = 'hello';
greeting.test = 'foo';
greeting.test; // undefined (therefore, not object)

```

**Creating an object**
In JavaScript, an object can be created in two ways:

=>**Object literal**
The object literal is a simple way of creating an object using { } brackets. You can include key-value pair in { }, where key would be property or method name and value will be value of property of any data type or a function. Use comma (,) to separate multiple key-value pairs.

**syntax**
```js
var object-name = { key1: value1, key2: value2,... keyN: valueN};
```
**example**
```js
var emptyObject = {}; // object with no properties or methods

var person = { firstName: "John" }; // object with single property

// object with single method
var message = { 
                showMessage: function (val) { 
                            alert(val); 
                } 
            }; 

// object with properties & method
var person = { 
                firstName: "James", 
                lastName: "Bond", 
                age: 15, 
                getFullName: function () { 
                        return this.firstName + ' ' + this.lastName 
                }
            }; 
```
=> **Object Constructor**
The second way to create an object is with Object Constructor using **new** keyword. You can attach properties and methods using dot notation. Optionally, you can also create properties using [ ] brackets and specifying property name as string.

**example**
```js
var person = new Object();

// Attach properties and methods to person object     
person.firstName = "James";
person["lastName"] = "Bond"; 
person.age = 25;
person.getFullName = function () {
        return this.firstName + ' ' + this.lastName;
    };

// access properties & methods 
person.firstName; // James
person.lastName; // Bond
person.getFullName(); // James Bon
```


**How to access a value of a particular key in an object**
We can do this by 2 methods .
=> **Dot notation**

**syntax**
```js
objectName.keyName 
```

**example**
```js
var course = {  
	name: "GRA 2032",  
	start: 8,  
	end: 10  
} 
​  
course.name;

//GRA 2032
```
=> **Bracket Notation**
Or you can use bracket notation with the name of the key inside a string inside square brackets [""]

**syntax**
```js
objectName["keyName"]
```
**example**
```js
var course = {  
		name: "GRA 2032",  
		start: 8,  
		end: 10  
	}; 
​  
course["name"];
//GRA 2032

```
#### Setting keys

=> To add keys to an object or overwrite its keys, you have the same two options as  _getting_  its keys.  
You can use dot notation with the name of the key after a period . and an equals sign =.
```js
**example**

var character = {  
		name: "Donna",  
		hair: "red"  
	}
​  character.hair = "blonde";  
​ 
character;

// {  
"name": "Donna",  
"hair": "blonde"  
}
```
=> Or you can use bracket notation with the name of the key inside a string inside square brackets [""] and an equals sign =.
```
**example**
var character = {  
		name: "Donna",  
		hair: "red"  
		}
character["hair"] = "blonde";  
character;  
//{  
"name": "Donna",  
"hair": "blonde"  
}
```









