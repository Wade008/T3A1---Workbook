# **T3A1 - Workbook**  
**Name:** Wade Doolan  
**Student number:** 12678  

<hr>   

## **Question 1:**  

*Provide an overview and description of a standard source control process for a large project*  





<hr>

## **Question 2:**  

*What are the most important aspects of quality software?*

Quality software can be broadly defined as the extent to which the system meets the needs of the end users. Furthermore, these needs are listed in ISO/IEC 25010 and include the attributes shown below (Iso25000.com, 2022).

1. Functional suitability: is an important quality characteristic that represents how well a software product meets the explicit and implicit needs of its users. This quality characteristic has three sub-attributes:
    - *Functional completeness*, which relates to the degree to which the system provides all the functions stipulated by the users.
    - *Functional correctness*, pertains to the ability of the system to produce the correct results with the right amount of precision.
    - *Functional Appropriateness*, is the capacity of the software only run the functions necessary to achieve the tasks required by the users.     

(Iso25000.com 2022; Super User 2022)

2. Performance efficiency: relates to the performance of the system relative to the size of the resources used under certain conditions. The quality characteristic it comprised of a number sub-attributes:
    - *Time behaviour* is essentially the time it takes for the system to execute its functions. Faster processing time is typically more desirable.
    - *Use of resources* relates to the amount of resources used by the software product when performing tasks. Minimal use of resources like memory and storage to achieve desired outcomes is desirable.  
    - *Capacity* involves the maximum limit of the product and how well this meets the system requirements.
    
(Iso25000.com 2022; Kaur, Grover and Dixit 2018)






![quality software attributes](https://iso25000.com/images/figures/en/iso25010.png)

<hr>

## **Question 3:**  

*Outline a standard high level structure for a MERN stack application and explain the components*

<hr>

## **Question 4:**  

*A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?*


<hr>

## **Question 5:**  

*With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges*  




<hr>

## **Question 6:**  

*With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature*  


<hr>

## **Question 7:**  

*Explain control flow, using an example from the JavaScript programming language*

Control flow is the order in which code is executed by a computer. Without certain structures that can change the control flow, the computer will parse the code from the top line (left to right) to the bottom line of a script. However, the control flow of a program is frequently altered in order to achieve a desired outcome. Conditionals, loops and functions are the main structures used to change the flow of code (Mozilla.org, 2022b). 

Moreover, in JavaScript, block statements (code inside curly brackets ```{ code goes here }```) are used with the control flow statements to encapsulate the code that is executed based on the requirements of the conditional, loop or function. In addition to conditional, loop and function structures, JavaScript also includes structures that alter the control flow based on the detection of an error. The try...catch...finally statement is used to change the order in which code is read based on the detection of an error. This type of statement is typically used in combination with conditionals and functions (Mozilla.org, 2022c).

In JavaScript, function hoisting is another important concept to address when discussing control flow. When a function is declared in JavaScript, it is always read first and loaded into memory before any other code is executed. This means a function can be declared after it is called. Essentially, the control flow is altered to ensure a function is available to be called regardless of where it is declared in a script (JavaScript Tutorial, 2022).

### Example - conditionals 

As the name suggests, these structures alter a code's control flow based on whether a condition is met or not (Mozilla.org, 2022a). In JavaScript, conditionals can include:
- if...else statements
- switch statements
- Ternary operator  

(Mozilla.org, 2022e)

**Conditional control flow example**: Using the JavaScript example shown below:
1. The script's code is read from the top, with the object added into the variable ```myDetails```. 
2. The if ...else structure is then read, where the condition ```!myDetails.email``` is tested. That is, if there is no email value detected in the object ```myDetails``` (the condition is True), only the ``` console.log("Please enter a valid email")``` is executed and all the other code in the ```else``` section is ignored.
3. However, if an email value is detected in the object ```myDetails``` (the condition is False) then only the ```console.log("Email added successfully")``` is run and the code inside the ```if``` block is ignored. 
4. Essentially, the if ...else statement alters the control flow based on the result of the condition, with the aim of indicating if an email value has been added to the ```myDetails``` object.

(Mozilla.org, 2022e)  

JavaScript if ...else Example:

```js

const myDetails = {
    name: "Wade",
    phone: "1234567892",
    email: null
}

if (!myDetails.email) {
    console.log("Please enter a valid email")
} else {
    console.log("Email added successfully")
}

``` 
<hr>


## **Question 8:**  

*Explain type coercion, using examples from the JavaScript programming language*  

Type coercion is an implied process, where the code will automatically convert a value from one data type to another under certain circumstances (Mozilla.org, 2022f). For example, in JavaScript, a number value will be coerced into a string value when attempting to add a sting and a number together (see below).

**Example: General type coercion in JavaScript**
```js

let num1 = "5";
let num2 = 10;

let total = num1 + num2;

console.log(total)

// Will output 510 as a string

```
Notably, JavaScript is a weakly typed language, meaning the data type of a variable is determined when it is initialised with a value, not at declaration. Furthermore, type coercion in JavaScript occurs to the string, number and boolean primitive types. Importantly, how particular data types are coerced is dependent upon the type of operation being used (Bhalla, 2022).

1. String coercion  

As shown in the example above, a number is typically coerced into string when a number and string are added together. This also happens when a boolean and a string are added together (GeeksforGeeks, 2020).

 **JavaScript example: coercion to string type**

```js

let num1 = false;
let num2 = "22";

let total = num1 + num2;

console.log(total)

// Will output false22 as a string

```

2. Number coercion

Where possible, JavaScript will coerce a string to a number when operations like subtraction, multiplication, division and modulus are used between a number and string or two strings. If a string cannot be logically coerced into a number ```NaN``` is the result of the operation (GeeksforGeeks, 2020).

**JavaScript example: coercion to number type**

```js  

let num1 = 25;
let num2 = "5";

let result = num1 / num2;

console.log(result)

// Will output 5 as a number

```
JavaScript will also coerce Boolean values to numbers where appropriate. Since true can be represented a 1 and false as 0, it is logical for JavaScript to convert Boolean values to numeric values (GeeksforGeeks, 2020). The example below shows how this can happen.

**JavaScript example: coercion to number type**

```js


let num1 = true;
let num2 = false;
let num3 = true;

let result = num1 + num2 + num3;

console.log(result)


// Will output 2 as a number

```

3. The equality operator

When the non-strict equality operator ``` ( == ) ``` is used in JavaScript, non-number values will be coerced into numbers, where appropriate  However, coercion will not occur when the strict equality operator ```( === ) ``` is used (GeeksforGeeks, 2020). The example below shows how a string "12" is coerced into a number when it is compared to the number 12 using the non-strict equality operator.

**JavaScript example: equality operator**

```js


let num1 = 12;
let num2 = "12";


let result = num1 == num2

console.log(result)


// The output will be true

```

<hr>

## **Question 9:**

*Explain data types, using examples from the JavaScript programming language*

In programming, setting/knowing the type of data a variable holds (data type) is required for a computer to be able to perform operations on variables and solve certain problems. For example, for a computer to be able to multiply values together, it must be able to discern the information being multiplied together are numbers (W3schools.com, 2015b).  

JavaScript is a dynamically typed language meaning the same variable can be used to hold values with different data types. The example below shows how this can happen (W3schools.com 2015b; Mozilla.org 2022d).

```js

let myVar = 25; //myVar has Number data type
myVar = "First Name"; // myVar now has a String data type
myVar = true; // myVar now has a Boolean data type

```

JavaScript has eight basic data types, seven primitive and one non-primitive. A primitive data type in JavaScript is capable of holding only one single data (datum) while the non-primitive type (an Object) can hold collections of data (Programiz.com, 2022). JavaScript primitive types can be tested using the ``` typeof ``` except for the null data type. Null data types must be tested using ```=== null```. This is explained in the code below.  

```js

let a = 'string';
let b = 1;
let c;
let d = true;
let e = null;

console.log(typeof(a)) //outputs string
console.log(typeof(b)) //outputs number
console.log(typeof(c)) //output undefined   
console.log(typeof(d)) //outputs boolean
console.log(typeof(e)) //outputs object
console.log(e === null) //outputs true

```
### Examples of data types in JavaScript

The following are some examples of data types in JavaScript and what they're typically used for.  

- **Boolean type:** (primitive) A boolean type in JavaScript can hold two possibles values: true and false. This data type is typically used in situations that require a binary choice such as conditionals, for example, if...else or ternary operators.

- **Number type:** (primitive) A number type in JavaScript is able to hold integers and floating-point number values; however, there is a limit on the size of the number that can be stored. For example, JavaScript can hold a floating point number as a number type between $ \pm (2^{-1074} \text{ to } 2^{1024})$. And if a value is larger/smaller than the capacity it is converted to a default value. For example, if a positive value gets any larger than the size limit it is automatically converted to infinity. A number type is usually used for mathematical or counting operations. For example, a number type variable is used to count the number of iterations a for loop is required to perform. For example, ``` for(let i = 0; i < arr.length; i++) {Do something here...} ```, with i in this example a number data type used to count the number of iterations.

- **String type:** (primitive) A string type in JavaScript is used to hold text, with strings declared as words wrapped in inverted commas or back ticks (for string interpolation). For example, ``` let a = "string" ``` is the same as ``` let a = 'string' ```, which is the same as ``` let a = `string` ``` in that they all declare the variable ```a``` as a string data type. Importantly, each character in a string has an index position, allowing easy access to individual characters within string. For example, ``` let a = "string" console.log(a[0])``` will output the letter at index 0, in this case "s". 

(Mozilla.org 2022d; Programiz.com 2022)


<hr>  

## **Question 10:**

*Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language*  

In JavaScript, arrays are a special type of Oject that can hold a collection of values, which can be saved under a single name (W3schools.com, 2015a). For example, 
```js 
const names = ["Tom", "Andrew", "Jenny", "Peter"]
``` 
In terms of simple array manipulation, array elements are indexed starting at zero, which allows elements to be accessed, added or changed easily using square bracke notation (W3schools.com, 2015a). The example below shows how an array can be easily manipulated using index values:

```js  
const names = ["Tom", "Andrew", "Jenny", "Peter"]

//accessing an element at index[0]
console.log(names[1]) //outputs "Andrew"

//adding an element at index[4]
names[4]= "Alicia"
console.log(names) //outputs [ 'Tom', 'Andrew', 'Jenny', 'Peter', 'Alicia' ]

// changing an element value at index[0]
names[0] = "Rebecca"
console.log(names) //outputs [ 'Rebecca', 'Andrew', 'Jenny', 'Peter', 'Alicia' ]

```
Like most Objects in JavaScript, arrays come with properties and methods that can be used to manipulate arrays. In relation to array properties, the ```arr.length``` property can be used in structures like ```for ``` loops to iteratively access and manipulate an arrays elements (W3schools.com, 2015a).
 
```js

const names = ["Tom", "Andrew", "Jenny", "Peter"]

//using the length property to manipulate an array
for(let i = 0; i < names.length; i++) { 

    // add 'Hello my name is: ' to the front of each element
    names[i] = `Hello my name is: ${names[i]}`
}

console.log(names)

// outputs: [
//   'Hello my name is: Tom',
//   'Hello my name is: Andrew',
//   'Hello my name is: Jenny',
//   'Hello my name is: Peter'
// ]

```

However, JavaScript arrays also have an extensive list of methods that make array manipulation even easier. There are many array methods available in JavaScript, and it is outside the scope of this question to explore all of them. However, some of the more common array methods include ```join()```, ```push()```, ```pop()```, ```shift()```, ```unshift()```, ```map()``` and ```reduce()``` (Bolaji Ayodeji, 2019). An examples of each of these methods is shown below:

```js

const names = ["Tom", "Andrew", "Jenny", "Peter"]

// join()

// Join all the elements of an array into a single string based on a delimiter.
let allNames = names.join(" ")
console.log(allNames)
// outputs "Tom Andrew Jenny Peter" as a single string


// push()

// Push one or more elements onto the back of an array
names.push("Alex", "John")
console.log(names)
// outputs the names array with the names "Alex" and "John" added to the end of the array:
// [ 'Tom', 'Andrew', 'Jenny', 'Peter', 'Alex', 'John' ]


// pop()

// remove the last element from the back of an array
names.pop()
console.log(names)
// outputs the names array with "John" removed form the end of the array:
// [ 'Tom', 'Andrew', 'Jenny', 'Peter', 'Alex' ]


// shift()

// Remove the first element from the front of an array
names.shift()
console.log(names)
// outputs the names array with the first name removed from the array:
// [ 'Andrew', 'Jenny', 'Peter', 'Alex' ]


// unshift()

// Adds a new alement to the fron of an array
names.unshift("Tom")
console.log(names)
// outputs the names array with the name "Andrew" inserted at the front of the array.
//  [ 'Tom', 'Andrew', 'Jenny', 'Peter', 'Alex' ]


// map()

// builds a new array by manipulating the elements of another array.

let i = 1
const newNames = names.map(name => {

    let newName = `${name}_${i}`
    i++;
    return newName
})

console.log(newNames)
// outputs a new array (newNames), with each element including their position suffix.
// [ 'Tom_1', 'Andrew_2', 'Jenny_3', 'Peter_4', 'Alex_5' ]


// reduce()

// The reduce method can be used to calculate a single value from an array (e.g. a total value) from the elements in a numeric array 

salesData = [20, 40, 100, 300, 27, 86, 90, 578]

let totalSales = salesData.reduce((accumulatedValue, currentValue) => {
    return accumulatedValue + currentValue
}, 0)

console.log(totalSales)

// outputs 1241 

```
(Bolaji Ayodeji 2019; W3schools.com 2015a)


<hr>

## **Question 11:**

*Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language* 

In JavaScript, Objects are variables that contain a collection of values, with each value written as key:value pair. Notably, these key:value pairs are known as properties (W3schools.com, 2015c).

###  Creating objects

Objects can be declared in several ways by either 'object literal' syntax or using 'object constructor' syntax (Md. Abu Talha, 2018). Examples of several approaches are show below:

```js
//Object literal
const employee = {};

employee["firstname"] = "Tom";
employee["lastename"] = "Anderson";
employee["email"] = "t@2.com";
employee["phone"] = "0451236987";


console.log(employee)
// outputs {
//     firstname: 'Tom',
//     lastename: 'Anderson',
//     email: 't@2.com',
//     phone: '0451236987'
//   }

// ------------------------------------------------

// Object constructor

const employee = new Object();


employee.firstname = "Tom";
employee.lastename = "Anderson";
employee.email = "t@2.com";
employee.phone = "0451236987";


console.log(employee)
// outputs {
//     firstname: 'Tom',
//     lastename: 'Anderson',
//     email: 't@2.com',
//     phone: '0451236987'
//   }

// ------------------------------------------------


// Constructor function

function Employee(firstname, lastname, email, phone) {
    this.firstname = firstname
    this.lastname = lastname
    this.email = email
    this.phone = phone
}

let employee1 = new Employee("Tom", "Anderson", "t@2.com", "0451236987")

console.log(employee1)

// outputs 
// Employee {
//     firstname: 'Tom',
//     lastname: 'Anderson',
//     email: 't@2.com',
//     phone: '0451236987'
//   }
  
```

(Md. Abu Talha, 2018)
### Accessing, updating and deleting object properties

The properties within a JavaScript object can be accessed, altered or deleted using either bracket ```object[keyname]``` or dot ```object.keyname``` notation. The examples below show how object properties can be access, changed and deleted using both methods (Md. Abu Talha 2018; W3schools.com 2015c; W3schools.com 2022).

```js

// Using the employee1 object from the above example

// Accessing an object property value 

console.log(`${employee1.firstname}'s phone number is ${employee1.phone}`)

// outputs Tom's phone number is 0451236987


// Changing an object property value

employee1["email"] = "tom@3.com";

console.log(`${employee1["firstname"]}'s new email address is ${employee1["email"]}`)

// outputs Tom's new email address is tom@3.com

// Deleting an object property

delete employee1.email

console.log(employee1)

// outputs Employee {
//   firstname: 'Tom',
//   lastname: 'Anderson',
//   phone: '0451236987'
// }

```
(Md. Abu Talha 2018; W3schools.com 2015c; W3schools.com 2022)

### Merging objects

JavaScript objects can be merged by either using the spread operator ``` ...object``` or the ```object.assign()``` method (Md. Abu Talha, 2018). See examples below.

```js

// Merging two objects using the spread operator

const vehicle1 = {
    make: "Audi",
    model: "A4",
    body: "Sedan"
}

const vehicleColour = {
    colour:"Black"
}

const vehicleMerged = {
    ...vehicle1,
    ...vehicleColour
}

console.log(vehicleMerged)
// outputs { make: 'Audi', model: 'A4', body: 'Sedan', colour: 'Black' }


// Merging two objects using the Object.assign() method

const vehicle1 = {
    make: "Audi",
    model: "A4",
    body: "Sedan"
}

const vehicleColour = {
    colour:"Black"
}

const vehicleMerged = Object.assign(vehicle1, vehicleColour)
console.log(vehicleMerged)
// outputs { make: 'Audi', model: 'A4', body: 'Sedan', colour: 'Black' }

```
(Md. Abu Talha, 2018)

### Object keys, values and entries

JavaScript objects can also be manipulated by accessing their keys, values or entries (keys and values) and converting them into arrays. This is done using the ```Object.keys()```, ```Object.values()```, or the ```Object.entries()``` methods. The examples below show how these methods can be used (Md. Abu Talha, 2018).

```js

const vehicle1 = {
    make: "Audi",
    model: "A4",
    body: "Sedan",
    colour: "Black"
}

// Accessing an object's keys

const vehicle1Keys = Object.keys(vehicle1)
console.log(vehicle1Keys)
// outputs [ 'make', 'model', 'body', 'colour' ]


// Accessing an object's values

const vehicle1Value = Object.values(vehicle1)
console.log(vehicle1Value)
// outputs [ 'Audi', 'A4', 'Sedan', 'Black' ]

// Accessing an object's entries - producing a 2 dimensional array

const vehicle1Entries = Object.entries(vehicle1)
console.log(vehicle1Entries)
// outputs [[ 'make', 'Audi' ],[ 'model', 'A4' ],[ 'body', 'Sedan' ],[ 'colour', 'Black' ]]

```
(Md. Abu Talha, 2018).  

### Adding object methods

JavaScript also allow bespoke methods to be added to objects. See the example below (W3schools.com, 2015c).

```js



const customer1 = {
    firstname: "Kelly",
    lastname: "Clarkson",
    email: "k@C.com",
    phone: "1234567891",
    hello: function() {
        return `Hi, my name is ${this.firstname} ${this.lastname}`
    }
}

console.log(customer1.hello())
// outputs "Hi, my name is Kelly Clarkson"

```
(W3schools.com, 2015c)

<hr>

## **Question 12:**

*Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language*  



<hr>

## **Question 13:**

*For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes* 




<hr>



## References  



