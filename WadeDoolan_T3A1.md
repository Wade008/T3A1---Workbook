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

*Add short para re brief description of conditionals, loop sand functions. Mention hoisting for functions*

### Example - conditionals 

As the name suggests, these structures alter a code's control flow based on whether a condition is met or not (Mozilla.org, 2022b). In JavaScript, conditionals include:
- if...else statements
- switch statements
- Ternary operator  

(Mozilla.org, 2022c)

**Conditional control flow example**: Using the JavaScript example below:
1. The script's code is read from the top, with the object added into the variable ```myDetails```. 
2. The if ...else structure is then read, where the condition ```!myDetails.email``` is tested. That is, if there is no email value detected in the object ```myDetails``` (the condition is True), only the ``` console.log("Please enter a valid email")``` is executed and all the other code in the ```else``` section is ignored.
3. However, if an email value is detected in the object ```myDetails``` (the condition is False) then only the ```console.log("Email added successfully")``` and code inside the ```if``` block is ignored. 
4. Essentially, the if ...else statement alters the control flow based on the result of the condition, with the aim of indicating if an email value has been added to the ```myDetails``` object.

(Mozilla.org, 2022a)  

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
### Loops





### Functions


<hr>

## **Question 8:**  

*Explain type coercion, using examples from the JavaScript programming language* 

<hr>

## **Question 9:**

*Explain data types, using examples from the JavaScript programming language*


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



