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

```javascript  

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
```javascript

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

```javascript

let num1 = false;
let num2 = "22";

let total = num1 + num2;

console.log(total)

// Will output false22 as a string

```

2. Number coercion

Where possible, JavaScript will coerce a string to a number when operations like subtraction, multiplication, division and modulus are used between a number and string or two strings. If a string cannot be logically coerced into a number ```NaN``` is the result of the operation (GeeksforGeeks, 2020).

**JavaScript example: coercion to number type**

```javascript

let num1 = 25;
let num2 = "5";

let result = num1 / num2;

console.log(result)

// Will output 5 as a number

```
JavaScript will also coerce Boolean values to numbers where appropriate. Since true can be represented a 1 and false as 0, it is logical for JavaScript to convert Boolean values to numeric values (GeeksforGeeks, 2020). The example below shows how this can happen.

**JavaScript example: coercion to number type**

```javascript


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

```javascript


let num1 = 12;
let num2 = "12";


let result = num1 == num2

console.log(result)


// The output will be true

```

<hr>

## **Question 9:**

*Explain data types, using examples from the JavaScript programming language*

In programming, setting/knowing the type of data a variable holds (data type) is required for a computer to be able to perform operations on variables and solve certain problems. For example, for a computer to be able to multiply values together, it must be able to discern the information being multiplied together are numbers (W3schools.com, 2015).  

JavaScript is a dynamically typed language meaning the same variable can be used to hold values with different data types. The example below shows how this can happen (W3schools.com 2015; Mozilla.org 2022d).

```javascript

let myVar = 25; //myVar has Number data type
myVar = "First Name"; // myVar now has a String data type
myVar = true; // myVar now has a Boolean data type

```

JavaScript has seven basic data types, seven primitive and one non-primitive. A primitive data type in JavaScript is capable of holding only one single data while the non-primitive type (an Object) can hold collections of data (Programiz.com, 2022).   

Show examples for three data types 2 primitive and one object. Discuss how an array is an Object etc. 



(Mozilla.org, 2022d)

(Programiz.com, 2022)

(W3schools.com, 2015)


<hr>  

## **Question 10:**

*Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language*  



<hr>

## **Question 11:**

*Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language* 



<hr>

## **Question 12:**

*Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language*  



<hr>

## **Question 13:**

*For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognise and identify functions, ranges and classes* 




<hr>



## References  



