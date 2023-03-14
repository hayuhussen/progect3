# progect3
# javascript

javascript

variable in javascript

Variable means anything that can vary. In JavaScript, a variable stores data that can be changed later on.

In JavaScript, a variable can be declared using `var`, `let`, `const` keywords.

- **var** keyword is used to declare variables since JavaScript was created. It is confusing and error-prone when using variables declared using `var`.
- **let** keyword removes the confusion and error of `var`. It is the new and recommended way of declaring variables in JavaScript.
- **const** keyword is used to declare a constant variable that cannot be changed once assigned a value.
- Example: Variable Declaration

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Variables </h1>
<p id="p1"></p>
<script>
	let msg;

	document.getElementById("p1").innerHTML = msg;
</script>
</body>
</html>

```

-Datatype

In JavaScript, you can assign different types of values (data) to a variable e.g. string, number, boolean, etc.

Example: A Variable with Different Types of Data

<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Variables </h1>

```
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>

<script>
	let myvariable = 1;  // numeric value
	document.getElementById("p1").textContent = myvariable;

	myvariable = 'one'; // string value
	document.getElementById("p2").textContent = myvariable;

	myvariable = true; // Boolean value
	document.getElementById("p3").textContent = myvariable;
</script>
</body>
</html>
```

they are differnce tyep of datatype 1,primative ,datastructure datatype

-DataStructure

-Control stat

*if/else/swich

# JavaScript if...else Statements

JavaScript includes if/else conditional statements to control the program flow, similar to other programming languages.

JavaScript includes following forms of if-else statements:

1. if Statement
2. if else Statement
3. else if Statement
4. 

# if Statement

Use if conditional statement if you want to execute something based on some condition.

Example: if condition

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: if condition</h1>
<script>
	if( 1 > 0)
	{
		alert("1 is greater than 0");
	}

	if( 1 < 0)
	{
		alert("1 is less than 0");
	}
</script>
</body>
</html>

```

# else condition

Use else statement when you want to execute the code every time when if condition evaluates to false.

The else statement must follow **if** or **else if** statement. Multiple else block is NOT allowed.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: if-else condition</h1>
<script>
	var mySal = 500;
	var yourSal = 1000;

	if( mySal > yourSal)
	{
		alert("My Salary is greater than your salary");
	}
	else
	{
		alert("My Salary is less than or equal to your salary");
	}

</script>
</body>
</html>

```

# JavaScript switch

The **switch** is a conditional statement like if statement. Switch is useful when you want to execute one of the multiple code blocks based on the return value of a specified expression.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: switch case</h1>
<script>
	var a = 3;

	switch (a) {
		case 1:
			alert('case 1 executed');
		case 2:
			alert("case 2 executed");
			break;
	   case 3:
			alert("case 3 executed");
			break;
		case 4:
			alert("case 4 executed");
			break;
		default:
			alert("default case executed");
	}

</script>
</body>
</html>
```

-loop

*for loop

# JavaScript for Loop

JavaScript includes for loop like Java or C#. Use for loop to execute code repeatedly.

*Do while

-function

The for loop requires following three parts.

- Initializer: Initialize a counter variable to start with
- Condition: specify a condition that must evaluate to true for next iteration
- Iteration: increase or decrease counter

# **Control Statements in JavaScript**

Control statements are used to control the flow of execution of a program in JavaScript.**Conditional Statements**Conditional statements are used to execute a block of code only if a certain condition is met. There are two types of conditional statements in JavaScript:**if...else Statement**The **if...else** statement is used to execute a block of code if a condition is true and another block of code if the condition is false. The syntax is as follows:if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}

Plain Text**switch Statement**The **switch** statement is used to execute different actions based on different conditions. The syntax is as follows:switch (expression) {
  case value1:
    // code to be executed if expression matches value1
    break;
  case value2:
    // code to be executed if expression matches value2
    break;
  ...
  default:
    // code to be executed if expression doesn't match any of the values
}

Plain Text**Looping Statements**Looping statements are used to execute a block of code repeatedly as long as a certain condition is true. There are three types of looping statements in JavaScript:**for Loop**The **for** loop is used to execute a block of code a fixed number of times. The syntax is as follows:for (initialization; condition; increment/decrement) {
  // code to be executed
}

Plain Text**while Loop**The **while** loop is used to execute a block of code as long as a condition is true. The syntax is as follows:while (condition) {
  // code to be executed
}

Plain Text**do...while Loop**The **do...while** loop is used to execute a block of code at least once, and then repeats the loop as long as a condition is true. The syntax is as follows:do {
  // code to be executed
} while (condition);

Plain Text**Conclusion**Control statements are a fundamental part of programming in JavaScript. They allow you to control the flow of execution of your program and make it more efficient and effective. By understanding the different types of control statements, you can write better code and become a more proficient JavaScript programmer.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: for loop</h1>
<p id="p0"></p>
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>
<p id="p4"></p>
<script>
	for (var i = 0; i < 5; i++)
	{
		document.getElementById("p" + i).innerHTML = i;
	}
</script>
</body>
</html>

```

In JavaScript, an object is a collection of key-value pairs, where each key is a string (or symbol) and each value can be any data type. Objects are used to represent real-world entities, such as a person, a car, or a book.

## Object Literal

The easiest way to create an object is by using the object literal notation, which is a comma-separated list of name-value pairs enclosed in curly braces. Here is an example of an object that represents a person:

```
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

```

You can access the properties of an object using the dot notation or the bracket notation. Here are some examples:

```
console.log(person.name); // "John"
console.log(person["age"]); // 30

```

## Object Constructor

Another way to create an object is by using the Object constructor function. Here is an example:

```
const person = new Object();
person.name = "John";
person.age = 30;
person.city = "New York";

```

You can also use the Object constructor function to create an object that inherits from another object. Here is an example:

```
const person = new Object();
person.name = "John";
person.age = 30;
person.city = "New York";

const employee = new Object(person);
employee.salary = 50000;

```

In this example, the `employee` object inherits the properties of the `person` object.

## Object Methods

An object can also have methods, which are functions that are associated with the object. Here is an example of an object that represents a calculator:

```
const calculator = {
  add: function(a, b) {
    return a + b;
  },
  subtract: function(a, b) {
    return a - b;
  }
};

```

You can call the methods of an object using the dot notation. Here are some examples:

```
console.log(calculator.add(2, 3)); // 5
console.log(calculator.subtract(5, 3)); // 2

```

## Object Prototypes

In JavaScript, all objects inherit from a prototype object. You can add properties and methods to the prototype object, and those properties and methods will be available to all objects that inherit from the prototype. Here is an example:

```
function Person(name, age, city) {
  this.name = name;
  this.age = age;
  this.city = city;
}

Person.prototype.greet = function() {
  console.log(`Hello, my name is ${this.name}`);
};

const person = new Person("John", 30, "New York");
person.greet(); // "Hello, my name is John"

```

In this example, the `Person` function is used as a constructor to create a new object that represents a person. The `greet` method is added to the prototype object of the `Person` function, so that all objects that are created using the `Person` constructor will have access to the `greet` method.

**JavaScript Objects: Create Objects, Access Properties & Methods**

An object is a non-primitive, structured data type in JavaScript. Objects are same as variables in JavaScript, the only difference is that an object holds multiple values in terms of properties and methods.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Object</h1>
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>
<p id="p4"></p>
<p id="p5"></p>
<script>
	var person = new Object();

	// Attach properties and methods to person object
	person.firstName = "James";
	person["lastName"] = "Bond";
	person.age = 25;
	person.getFullName = function () {
			return this.firstName + ' ' + this.lastName;
		};

	// access properties & methods
	document.getElementById("p1").innerHTML = person.firstName;
	document.getElementById("p2").innerHTML = person.lastName;

	document.getElementById("p3").innerHTML = person["firstName"];
	document.getElementById("p4").innerHTML = person["lastName"];

	document.getElementById("p5").innerHTML = person.getFullName();

</script>
</body>
</html>
```

# Functions in JavaScript

Functions are the basic building block of JavaScript. Functions allow us to encapsulate a block of code and reuse it multiple times.

Functions make JavaScript code more readable, organized, reusable, and maintainable

- <!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript function</h1>
<script>
	function greet() {
		alert("Hello World!");
	}

	greet();
</script>
</body>
</html>
    
    
    A JavaScript function is a block of code designed to perform a particular task.
    
    A JavaScript function is executed when "something" invokes it (calls it).
    
    **<!DOCTYPE html>
    <html>
    <body>**
    
    **<h2>JavaScript Functions</h2>**
    
    **<p>This example calls a function which performs a calculation, and returns the result:</p>**
    
    **<p id="demo"></p>**
    
    **<script>
    function myFunction(p1, p2) {
    return p1 * p2;
    }
    document.getElementById("demo").innerHTML = myFunction(4, 3);
    </script>**
    
    **</body>
    </html>**
    
    function
    
    *name*
    
    (
    
    *parameter1, parameter2, parameter3*
    
    ) {
    
    //
    
    *code to be executed*
    
    }
    
    Function **parameters** are listed inside the parentheses () in the function definition.
    
    Function **arguments** are the **values** received by the function when it is invoked.
    
    Inside the function, the arguments (the parameters) behave as local variables.
    
    ---
    
    # Function Invocation
    
    The code inside the function will execute when "something" **invokes** (calls) the function:
    
    - When an event occurs (when a user clicks a button)
    - When it is invoked (called) from JavaScript code
    - Automatically (self invoked)
    
    # JavaScript Function Syntax
    
    A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.
    
    Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
    
    The parentheses may include parameter names separated by commas:**(*parameter1, parameter2, ...*)**
    
    The code to be executed, by the function, is placed inside curly brackets: **{}**
    
    # JavaScript Events
    
    ---
    
    HTML events are **"things"** that happen to HTML elements.
    
    When JavaScript is used in HTML pages, JavaScript can **"react"** on these events.
    
    ---
    
    # HTML Events
    
    An HTML event can be something the browser does, or something a user does.
    
    Here are some examples of HTML events:
    
    - An HTML web page has finished loading
    - An HTML input field was changed
    - An HTML button was clicked
    
    Often, when events happen, you may want to do something.
    
    JavaScript lets you execute code when events are detected.
    
    HTML allows event handler attributes, **with JavaScript code**, to be added to HTML elements.
    
    With single quotes:
    
    <*element* *event*=**'*some JavaScript*'**>
    
    With double quotes:
    
    <*element* *event*=**"*some JavaScript*"**>
    
    In the following example, an `onclick` attribute (with code), is added to a `<button>` element:
    
    # Example
    
    <button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
    

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

<!DOCTYPE html>
<html>
<body>

<button onclick="document.getElementById('demo').innerHTML=Date()">The time is?</button>

<p id="demo"></p>

</body>
</html>

# vaScript Event Handlers

Event handlers can be used to handle and verify user input, user actions, and browser actions:

- Things that should be done every time a page loads
- Things that should be done when the page is closed
- Action that should be performed when a user clicks a button
- Content that should be verified when a user inputs data
- And more ...

Many different methods can be used to let JavaScript work with events:

- HTML event attributes can execute JavaScript code directly
- HTML event attributes can call JavaScript functions
- You can assign your own event handler functions to HTML elements
- You can prevent events from being sent or being handled
- And more ...

# **JSON in JavaScript**

JSON stands for **JavaScript Object Notation**, which is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others.JSON has become a popular format for data exchange between web services, and is frequently used to transmit data between a server and a web application, as an alternative to XML.In JavaScript, you can work with JSON data using built-in methods such as JSON.parse() and JSON.stringify().The JSON.parse() method is used to convert a JSON string into a JavaScript object:

Here's an example of using JSON in JavaScript:

```
// a JSON object
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the JSON object to a string
const personString = JSON.stringify(person);

// output the string
console.log(personString);

// convert the string back to a JSON object
const personObject = JSON.parse(personString);

// output the object
console.log(personObject);

```

In JavaScript, there are two types of storage options available for storing data in the browser:

1. **Local Storage**: The data stored in local storage persists even after the browser is closed. It can be accessed by any page from the same domain that uses the same storage mechanism.
2. **Session Storage**: The data stored in session storage is available only for the duration of the browser session. Once the browser is closed, the data is lost. Session storage is available only to the page that created it.

Both local storage and session storage can be used to store data as key-value pairs. JSON can be used to store complex objects in these storage mechanisms.

Here's an example of storing data in local storage using JSON:

```
// create an object to store
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the object to a string using JSON.stringify()
const personString = JSON.stringify(person);

// store the string in local storage
localStorage.setItem("person", personString);

// retrieve the string from local storage
const retrievedPersonString = localStorage.getItem("person");

// convert the string back to an object using JSON.parse()
const retrievedPerson = JSON.parse(retrievedPersonString);

// output the retrieved object
console.log(retrievedPerson);

```

In this example, we create an object called `person` and convert it to a string using `JSON.stringify()`. We then store the string in local storage using `localStorage.setItem()`. To retrieve the object from local storage, we use `localStorage.getItem()` to get the string, and then use `JSON.parse()` to convert the string back to an object. Finally, we output the retrieved object to the console.

JSON data can be stored in both internal and external storage in JavaScript.

**Internal Storage:**

Internal storage in JavaScript refers to the browser's `localStorage` and `sessionStorage` objects, which allow you to store data on the client-side. `localStorage` allows you to store data that persists even after the browser is closed, while `sessionStorage` allows you to store data that is only available during the current session.

Here's an example of storing JSON data in `localStorage`:

```
// create a JavaScript object
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the object to a JSON string
const personString = JSON.stringify(person);

// store the string in local storage
localStorage.setItem("person", personString);

```

In this example, we create a JavaScript object called `person` that contains three properties: `name`, `age`, and `city`. We then use the `JSON.stringify()` method to convert the object into a string, which can be stored in `localStorage` using the `localStorage.setItem()` method.

To retrieve the data from `localStorage` and convert it back into a JavaScript object, we use the `localStorage.getItem()` method to get the string, and then use the `JSON.parse()` method to convert the string back into an object:

```
// retrieve the string from local storage
const personString = localStorage.getItem("person");

// convert the string back to an object
const person = JSON.parse(personString);

```

**External Storage:**

External storage in JavaScript refers to storing data on a server and retrieving it using AJAX. In this case, the data is typically returned in JSON format.

Here's an example of retrieving JSON data from a server using AJAX:

```
// retrieve data from server using AJAX
const xhr = new XMLHttpRequest();
xhr.open("GET", "<https://example.com/data.json>");

xhr.onload = function() {
  if (xhr.status === 200) {
    // parse JSON data into a JavaScript object
    const data = JSON.parse(xhr.responseText);

    // do something with the data
    console.log(data);
  }
};

xhr.send();

```

In this example, we use the `XMLHttpRequest` object to retrieve data from a server in JSON format. Once we have the data, we use the `JSON.parse()` method to convert the JSON string into a JavaScript object. We can then do whatever we want with the data, such as displaying it on a web page or using it to update the state of a JavaScript application.

These examples demonstrate how JSON can be used with both internal and external storage in JavaScript to create dynamic web applications.

In this example, we create a JSON object called "person" that contains three properties: "name", "age", and "city". We then use the JSON.stringify() method to convert the object into a string, which can be sent over the network or saved to a file. We output the string to the console.

Next, we use the JSON.parse() method to convert the string back into a JSON object. We output the object to the console, confirming that we have successfully converted the string back into an object.

json how to content store

json storage,promise and codeback

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can interact with the page. Nodes can have event handlers attached to them. Once an event is triggered, the event handlers get executed.

The **Document Object Model**
 (*DOM*
) is the data representation of the objects that comprise the structure and content of a document on the web. This guide will introduce the DOM, look at how the DOM represents an [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML)
 document in memory and how to use APIs to create web content and applications.

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

A web page is a document that can be either displayed in the browser window or as the HTML source. In both cases, it is the same document but the Document Object Model (DOM) representation allows it to be manipulated. As an object-oriented representation of the web page, it can be modified with a scripting language such as JavaScript.

For example, the DOM specifies that the `querySelectorAll` method in this code snippet must return a list of all the `[<p>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)` elements in the document:

To fetch a JSON object in JavaScript, you can use the built-in `fetch()` function. Here is an example:

```
fetch('<https://example.com/data.json>')
  .then(response => response.json())
  .then(data => console.log(data));

```

In this example, we use the `fetch()` function to retrieve a JSON file from a server. The `fetch()` function returns a `Promise` object, which we can use to access the response data. We then call the `json()` method on the response object to convert the response data into a JSON object. Finally, we use the `then()` method to access the JSON data.

Note that the `fetch()` function is asynchronous, so you may need to use `async/await` or callbacks to handle the response data.

HTML5 web Storage they are 2 part session storage and local storage

To remove a child element from a JSON object in JavaScript, you can use the `delete` keyword followed by the name of the property you want to remove. Here is an example:

```
// create a JSON object
const person = {
  name: 'John',
  age: 30,
  city: 'New York'
};

// remove the 'city' property
delete person.city;

```

In this example, we create a JSON object called `person` that contains three properties: `name`, `age`, and `city`. To remove the `city` property from the object, we use the `delete` keyword followed by `person.city`. Note that this will permanently remove the `city` property from the object.

[variable &Data type in javascript (1)](https://www.notion.so/variable-Data-type-in-javascript-1-de5ae553df614c40b4c23ec642c0a6d8)

[variable and Datatype in javascript (1)](https://www.notion.so/variable-and-Datatype-in-javascript-1-f928836a926d44e1a616e80e2c3376aa)

[](https://www.notion.so/073c9f9865364cf9b390d783fc478a09)

javascript

variable in javascript

Variable means anything that can vary. In JavaScript, a variable stores data that can be changed later on.

In JavaScript, a variable can be declared using `var`, `let`, `const` keywords.

- **var** keyword is used to declare variables since JavaScript was created. It is confusing and error-prone when using variables declared using `var`.
- **let** keyword removes the confusion and error of `var`. It is the new and recommended way of declaring variables in JavaScript.
- **const** keyword is used to declare a constant variable that cannot be changed once assigned a value.
- Example: Variable Declaration

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Variables </h1>
<p id="p1"></p>
<script>
	let msg;

	document.getElementById("p1").innerHTML = msg;
</script>
</body>
</html>

```

-Datatype

In JavaScript, you can assign different types of values (data) to a variable e.g. string, number, boolean, etc.

Example: A Variable with Different Types of Data

<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Variables </h1>

```
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>

<script>
	let myvariable = 1;  // numeric value
	document.getElementById("p1").textContent = myvariable;

	myvariable = 'one'; // string value
	document.getElementById("p2").textContent = myvariable;

	myvariable = true; // Boolean value
	document.getElementById("p3").textContent = myvariable;
</script>
</body>
</html>
```

they are differnce tyep of datatype 1,primative ,datastructure datatype

-DataStructure

-Control stat

*if/else/swich

# JavaScript if...else Statements

JavaScript includes if/else conditional statements to control the program flow, similar to other programming languages.

JavaScript includes following forms of if-else statements:

1. if Statement
2. if else Statement
3. else if Statement
4. 

# if Statement

Use if conditional statement if you want to execute something based on some condition.

Example: if condition

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: if condition</h1>
<script>
	if( 1 > 0)
	{
		alert("1 is greater than 0");
	}

	if( 1 < 0)
	{
		alert("1 is less than 0");
	}
</script>
</body>
</html>

```

# else condition

Use else statement when you want to execute the code every time when if condition evaluates to false.

The else statement must follow **if** or **else if** statement. Multiple else block is NOT allowed.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: if-else condition</h1>
<script>
	var mySal = 500;
	var yourSal = 1000;

	if( mySal > yourSal)
	{
		alert("My Salary is greater than your salary");
	}
	else
	{
		alert("My Salary is less than or equal to your salary");
	}

</script>
</body>
</html>

```

# JavaScript switch

The **switch** is a conditional statement like if statement. Switch is useful when you want to execute one of the multiple code blocks based on the return value of a specified expression.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: switch case</h1>
<script>
	var a = 3;

	switch (a) {
		case 1:
			alert('case 1 executed');
		case 2:
			alert("case 2 executed");
			break;
	   case 3:
			alert("case 3 executed");
			break;
		case 4:
			alert("case 4 executed");
			break;
		default:
			alert("default case executed");
	}

</script>
</body>
</html>
```

-loop

*for loop

# JavaScript for Loop

JavaScript includes for loop like Java or C#. Use for loop to execute code repeatedly.

*Do while

-function

The for loop requires following three parts.

- Initializer: Initialize a counter variable to start with
- Condition: specify a condition that must evaluate to true for next iteration
- Iteration: increase or decrease counter

# **Control Statements in JavaScript**

Control statements are used to control the flow of execution of a program in JavaScript.**Conditional Statements**Conditional statements are used to execute a block of code only if a certain condition is met. There are two types of conditional statements in JavaScript:**if...else Statement**The **if...else** statement is used to execute a block of code if a condition is true and another block of code if the condition is false. The syntax is as follows:if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}

Plain Text**switch Statement**The **switch** statement is used to execute different actions based on different conditions. The syntax is as follows:switch (expression) {
  case value1:
    // code to be executed if expression matches value1
    break;
  case value2:
    // code to be executed if expression matches value2
    break;
  ...
  default:
    // code to be executed if expression doesn't match any of the values
}

Plain Text**Looping Statements**Looping statements are used to execute a block of code repeatedly as long as a certain condition is true. There are three types of looping statements in JavaScript:**for Loop**The **for** loop is used to execute a block of code a fixed number of times. The syntax is as follows:for (initialization; condition; increment/decrement) {
  // code to be executed
}

Plain Text**while Loop**The **while** loop is used to execute a block of code as long as a condition is true. The syntax is as follows:while (condition) {
  // code to be executed
}

Plain Text**do...while Loop**The **do...while** loop is used to execute a block of code at least once, and then repeats the loop as long as a condition is true. The syntax is as follows:do {
  // code to be executed
} while (condition);

Plain Text**Conclusion**Control statements are a fundamental part of programming in JavaScript. They allow you to control the flow of execution of your program and make it more efficient and effective. By understanding the different types of control statements, you can write better code and become a more proficient JavaScript programmer.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: for loop</h1>
<p id="p0"></p>
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>
<p id="p4"></p>
<script>
	for (var i = 0; i < 5; i++)
	{
		document.getElementById("p" + i).innerHTML = i;
	}
</script>
</body>
</html>

```

In JavaScript, an object is a collection of key-value pairs, where each key is a string (or symbol) and each value can be any data type. Objects are used to represent real-world entities, such as a person, a car, or a book.

## Object Literal

The easiest way to create an object is by using the object literal notation, which is a comma-separated list of name-value pairs enclosed in curly braces. Here is an example of an object that represents a person:

```
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

```

You can access the properties of an object using the dot notation or the bracket notation. Here are some examples:

```
console.log(person.name); // "John"
console.log(person["age"]); // 30

```

## Object Constructor

Another way to create an object is by using the Object constructor function. Here is an example:

```
const person = new Object();
person.name = "John";
person.age = 30;
person.city = "New York";

```

You can also use the Object constructor function to create an object that inherits from another object. Here is an example:

```
const person = new Object();
person.name = "John";
person.age = 30;
person.city = "New York";

const employee = new Object(person);
employee.salary = 50000;

```

In this example, the `employee` object inherits the properties of the `person` object.

## Object Methods

An object can also have methods, which are functions that are associated with the object. Here is an example of an object that represents a calculator:

```
const calculator = {
  add: function(a, b) {
    return a + b;
  },
  subtract: function(a, b) {
    return a - b;
  }
};

```

You can call the methods of an object using the dot notation. Here are some examples:

```
console.log(calculator.add(2, 3)); // 5
console.log(calculator.subtract(5, 3)); // 2

```

## Object Prototypes

In JavaScript, all objects inherit from a prototype object. You can add properties and methods to the prototype object, and those properties and methods will be available to all objects that inherit from the prototype. Here is an example:

```
function Person(name, age, city) {
  this.name = name;
  this.age = age;
  this.city = city;
}

Person.prototype.greet = function() {
  console.log(`Hello, my name is ${this.name}`);
};

const person = new Person("John", 30, "New York");
person.greet(); // "Hello, my name is John"

```

In this example, the `Person` function is used as a constructor to create a new object that represents a person. The `greet` method is added to the prototype object of the `Person` function, so that all objects that are created using the `Person` constructor will have access to the `greet` method.

**JavaScript Objects: Create Objects, Access Properties & Methods**

An object is a non-primitive, structured data type in JavaScript. Objects are same as variables in JavaScript, the only difference is that an object holds multiple values in terms of properties and methods.

```
<!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript Object</h1>
<p id="p1"></p>
<p id="p2"></p>
<p id="p3"></p>
<p id="p4"></p>
<p id="p5"></p>
<script>
	var person = new Object();

	// Attach properties and methods to person object
	person.firstName = "James";
	person["lastName"] = "Bond";
	person.age = 25;
	person.getFullName = function () {
			return this.firstName + ' ' + this.lastName;
		};

	// access properties & methods
	document.getElementById("p1").innerHTML = person.firstName;
	document.getElementById("p2").innerHTML = person.lastName;

	document.getElementById("p3").innerHTML = person["firstName"];
	document.getElementById("p4").innerHTML = person["lastName"];

	document.getElementById("p5").innerHTML = person.getFullName();

</script>
</body>
</html>
```

# Functions in JavaScript

Functions are the basic building block of JavaScript. Functions allow us to encapsulate a block of code and reuse it multiple times.

Functions make JavaScript code more readable, organized, reusable, and maintainable

- <!DOCTYPE html>
<html>
<body>
<h1>Demo: JavaScript function</h1>
<script>
	function greet() {
		alert("Hello World!");
	}

	greet();
</script>
</body>
</html>
    
    
    A JavaScript function is a block of code designed to perform a particular task.
    
    A JavaScript function is executed when "something" invokes it (calls it).
    
    **<!DOCTYPE html>
    <html>
    <body>**
    
    **<h2>JavaScript Functions</h2>**
    
    **<p>This example calls a function which performs a calculation, and returns the result:</p>**
    
    **<p id="demo"></p>**
    
    **<script>
    function myFunction(p1, p2) {
    return p1 * p2;
    }
    document.getElementById("demo").innerHTML = myFunction(4, 3);
    </script>**
    
    **</body>
    </html>**
    
    function
    
    *name*
    
    (
    
    *parameter1, parameter2, parameter3*
    
    ) {
    
    //
    
    *code to be executed*
    
    }
    
    Function **parameters** are listed inside the parentheses () in the function definition.
    
    Function **arguments** are the **values** received by the function when it is invoked.
    
    Inside the function, the arguments (the parameters) behave as local variables.
    
    ---
    
    # Function Invocation
    
    The code inside the function will execute when "something" **invokes** (calls) the function:
    
    - When an event occurs (when a user clicks a button)
    - When it is invoked (called) from JavaScript code
    - Automatically (self invoked)
    
    # JavaScript Function Syntax
    
    A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.
    
    Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
    
    The parentheses may include parameter names separated by commas:**(*parameter1, parameter2, ...*)**
    
    The code to be executed, by the function, is placed inside curly brackets: **{}**
    
    # JavaScript Events
    
    ---
    
    HTML events are **"things"** that happen to HTML elements.
    
    When JavaScript is used in HTML pages, JavaScript can **"react"** on these events.
    
    ---
    
    # HTML Events
    
    An HTML event can be something the browser does, or something a user does.
    
    Here are some examples of HTML events:
    
    - An HTML web page has finished loading
    - An HTML input field was changed
    - An HTML button was clicked
    
    Often, when events happen, you may want to do something.
    
    JavaScript lets you execute code when events are detected.
    
    HTML allows event handler attributes, **with JavaScript code**, to be added to HTML elements.
    
    With single quotes:
    
    <*element* *event*=**'*some JavaScript*'**>
    
    With double quotes:
    
    <*element* *event*=**"*some JavaScript*"**>
    
    In the following example, an `onclick` attribute (with code), is added to a `<button>` element:
    
    # Example
    
    <button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
    

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

<!DOCTYPE html>
<html>
<body>

<button onclick="document.getElementById('demo').innerHTML=Date()">The time is?</button>

<p id="demo"></p>

</body>
</html>

# vaScript Event Handlers

Event handlers can be used to handle and verify user input, user actions, and browser actions:

- Things that should be done every time a page loads
- Things that should be done when the page is closed
- Action that should be performed when a user clicks a button
- Content that should be verified when a user inputs data
- And more ...

Many different methods can be used to let JavaScript work with events:

- HTML event attributes can execute JavaScript code directly
- HTML event attributes can call JavaScript functions
- You can assign your own event handler functions to HTML elements
- You can prevent events from being sent or being handled
- And more ...

# **JSON in JavaScript**

JSON stands for **JavaScript Object Notation**, which is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others.JSON has become a popular format for data exchange between web services, and is frequently used to transmit data between a server and a web application, as an alternative to XML.In JavaScript, you can work with JSON data using built-in methods such as JSON.parse() and JSON.stringify().The JSON.parse() method is used to convert a JSON string into a JavaScript object:

Here's an example of using JSON in JavaScript:

```
// a JSON object
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the JSON object to a string
const personString = JSON.stringify(person);

// output the string
console.log(personString);

// convert the string back to a JSON object
const personObject = JSON.parse(personString);

// output the object
console.log(personObject);

```

In JavaScript, there are two types of storage options available for storing data in the browser:

1. **Local Storage**: The data stored in local storage persists even after the browser is closed. It can be accessed by any page from the same domain that uses the same storage mechanism.
2. **Session Storage**: The data stored in session storage is available only for the duration of the browser session. Once the browser is closed, the data is lost. Session storage is available only to the page that created it.

Both local storage and session storage can be used to store data as key-value pairs. JSON can be used to store complex objects in these storage mechanisms.

Here's an example of storing data in local storage using JSON:

```
// create an object to store
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the object to a string using JSON.stringify()
const personString = JSON.stringify(person);

// store the string in local storage
localStorage.setItem("person", personString);

// retrieve the string from local storage
const retrievedPersonString = localStorage.getItem("person");

// convert the string back to an object using JSON.parse()
const retrievedPerson = JSON.parse(retrievedPersonString);

// output the retrieved object
console.log(retrievedPerson);

```

In this example, we create an object called `person` and convert it to a string using `JSON.stringify()`. We then store the string in local storage using `localStorage.setItem()`. To retrieve the object from local storage, we use `localStorage.getItem()` to get the string, and then use `JSON.parse()` to convert the string back to an object. Finally, we output the retrieved object to the console.

JSON data can be stored in both internal and external storage in JavaScript.

**Internal Storage:**

Internal storage in JavaScript refers to the browser's `localStorage` and `sessionStorage` objects, which allow you to store data on the client-side. `localStorage` allows you to store data that persists even after the browser is closed, while `sessionStorage` allows you to store data that is only available during the current session.

Here's an example of storing JSON data in `localStorage`:

```
// create a JavaScript object
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// convert the object to a JSON string
const personString = JSON.stringify(person);

// store the string in local storage
localStorage.setItem("person", personString);

```

In this example, we create a JavaScript object called `person` that contains three properties: `name`, `age`, and `city`. We then use the `JSON.stringify()` method to convert the object into a string, which can be stored in `localStorage` using the `localStorage.setItem()` method.

To retrieve the data from `localStorage` and convert it back into a JavaScript object, we use the `localStorage.getItem()` method to get the string, and then use the `JSON.parse()` method to convert the string back into an object:

```
// retrieve the string from local storage
const personString = localStorage.getItem("person");

// convert the string back to an object
const person = JSON.parse(personString);

```

**External Storage:**

External storage in JavaScript refers to storing data on a server and retrieving it using AJAX. In this case, the data is typically returned in JSON format.

Here's an example of retrieving JSON data from a server using AJAX:

```
// retrieve data from server using AJAX
const xhr = new XMLHttpRequest();
xhr.open("GET", "<https://example.com/data.json>");

xhr.onload = function() {
  if (xhr.status === 200) {
    // parse JSON data into a JavaScript object
    const data = JSON.parse(xhr.responseText);

    // do something with the data
    console.log(data);
  }
};

xhr.send();

```

In this example, we use the `XMLHttpRequest` object to retrieve data from a server in JSON format. Once we have the data, we use the `JSON.parse()` method to convert the JSON string into a JavaScript object. We can then do whatever we want with the data, such as displaying it on a web page or using it to update the state of a JavaScript application.

These examples demonstrate how JSON can be used with both internal and external storage in JavaScript to create dynamic web applications.

In this example, we create a JSON object called "person" that contains three properties: "name", "age", and "city". We then use the JSON.stringify() method to convert the object into a string, which can be sent over the network or saved to a file. We output the string to the console.

Next, we use the JSON.parse() method to convert the string back into a JSON object. We output the object to the console, confirming that we have successfully converted the string back into an object.

json how to content store

json storage,promise and codeback

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can interact with the page. Nodes can have event handlers attached to them. Once an event is triggered, the event handlers get executed.

The **Document Object Model**
 (*DOM*
) is the data representation of the objects that comprise the structure and content of a document on the web. This guide will introduce the DOM, look at how the DOM represents an [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML)
 document in memory and how to use APIs to create web content and applications.

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

A web page is a document that can be either displayed in the browser window or as the HTML source. In both cases, it is the same document but the Document Object Model (DOM) representation allows it to be manipulated. As an object-oriented representation of the web page, it can be modified with a scripting language such as JavaScript.

For example, the DOM specifies that the `querySelectorAll` method in this code snippet must return a list of all the `[<p>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)` elements in the document:

To fetch a JSON object in JavaScript, you can use the built-in `fetch()` function. Here is an example:

```
fetch('<https://example.com/data.json>')
  .then(response => response.json())
  .then(data => console.log(data));

```

In this example, we use the `fetch()` function to retrieve a JSON file from a server. The `fetch()` function returns a `Promise` object, which we can use to access the response data. We then call the `json()` method on the response object to convert the response data into a JSON object. Finally, we use the `then()` method to access the JSON data.

Note that the `fetch()` function is asynchronous, so you may need to use `async/await` or callbacks to handle the response data.

HTML5 web Storage they are 2 part session storage and local storage

To remove a child element from a JSON object in JavaScript, you can use the `delete` keyword followed by the name of the property you want to remove. Here is an example:

```
// create a JSON object
const person = {
  name: 'John',
  age: 30,
  city: 'New York'
};

// remove the 'city' property
delete person.city;

```

In this example, we create a JSON object called `person` that contains three properties: `name`, `age`, and `city`. To remove the `city` property from the object, we use the `delete` keyword followed by `person.city`. Note that this will permanently remove the `city` property from the object.

[variable &Data type in javascript (1)](https://www.notion.so/variable-Data-type-in-javascript-1-bfcb399341df42f48bd11ca1680ed43c)

[variable and Datatype in javascript (1)](https://www.notion.so/variable-and-Datatype-in-javascript-1-e1be025076af4872877bd2563dba4122)

[](https://www.notion.so/200a8ee5461e4300a4c0dffe36c011cd)
