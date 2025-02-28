1)  What is javascript ?
=> Javascript is a high level interpreted programming language primarly used for creating interactive web pages.

2) What are the different data types in javascript ?
=> Javascript supports various data types including string , numbers , booleans, null , undefined, sumbol and object (symbol added in es6);

3) How do you declare variables in javascript ?
=> Variables can be declared using the "let" "var" and "const" keywords;

4) What is the different between let var and const ?
=> var has function scope let has block scope and 'const' is used to declare constans whose value cannot be
reassigned

5) What is the use of == and === operators in javascript?
=> == is used for loose equality comparison whereas === is used for strict equality comparison, which compares both value and type.

6) How do you comment in javascript?
=> Single line comment we can achived by using // and for multi-line commends we can use /* */

7) What are javascript primitive data types?
=> Primitive data types in javascript include strings, numbers, boolearn, null, undefined, and symbols

8) what is typeof operator used for?
=> the typeof operator is used to determine the type of the variable or expression;

9) Explain hosting in javascript?
=> Hosting is a default behaviour of javascript that moves the variables and functions declaration to the top of their scope during compilation.

10) What is NaN in javascript?
=> NaN stands for Not-a-number and is a value returned when a mathematical operation cannot produce a meaningful result.

11) Explain closure in javascript?
=> 
// * 1) Lexical Scope: 
// ? Lexical scope means that a function can access variables from its own scope 
// ? parent scope and so on up the scope chain. the scope is determined at the time 
// ? the code is written (not when it runs )

// * 2) Closure:
// a closure is when a function remembers and keeps access to variables from it's 
// lexical scope, even after the parent functio has finished execution

12) What are higher order function in javascript?
=> Higher order function is a function that operators on other functions, either by taking them as an arguments or by returning them.


13) What is a callback function?
=> a callback function is a function passed as an argument to another function, which is then invoked inside the outer function to complete some kind of action;

14) What is event delegation in javascript?
=> Event delegation is a technique where a single event listener is attached to a parent element to listen for events that occurs on its children. This is particularly useFul when dealing with dynamically added elements.

15) Explain the concept of prototypal inheritence in javascript?
=> Prototype Inheritence is a feature of javascript where objects can (inherit properties and methods )from other objects using the prototype chain.

16) What is the this keyword in javascript?
=> Ok, so let's start by defining what the this keyword is. In JavaScript, the this keyword always refers to an object. The thing about it is that the object it refers to will vary depending on how and where this is being called.

17) How does javascript handles asynchronous task in javascript?
=> Javascript uses mechanisms such as callbacks, promises, and async-await to handle asynchronous operation.

18) What are javascript promises ?
=>  Promises are objects representing the eventual completion or failure of an asynchronous operation. and they allow for more readable and manageablea asynchronous code.

19) explain the null and undefined in javascript?
=> null represents the intentional absense of any object value, 
while undefined represents absense of defined value;

20) what is the event loop in javascript and how does it work ?
=> The event loop is a mechanism in javascript that handles asynchronous tasks. Javascript is single threaded so the event loop ensures non-blocking tasks (like setTimeout, Promises etc) are executed when the call stack is empty. it continuesly checks the call stack and task queues, processing tasks one by one.


21)  What are Microtasks and Macrotasks, and how are they scheduled in JavaScript?

=> Microtasks include Promises and process.nextTick, while Macrotasks include setTimeout, setImmediate, and I/O operations.
 Microtasks have higher priority and are executed right after the currently executing script, before any Macrotasks.

22) What is the difference between setTimeout, setImmediate, and process.nextTick?

=> setTimeout: Executes a callback after a specified delay.

setImmediate: Executes a callback after the current event loop cycle.

process.nextTick: Executes a callback before the next event loop cycle, giving it higher priority.

23) How does JavaScript handle asynchronous operations?

=> JavaScript handles asynchronous operations using Callbacks, Promises, and async/await. These allow non-blocking execution, ensuring smooth performance without freezing the main thread.

24)  What is a Promise, and how does it work under the hood?

=> A Promise is an object representing a future value. It can be in one of three states: pending, fulfilled, or rejected. Once a Promise is resolved or rejected, its associated .then() or .catch() handlers are executed asynchronously in the Microtask queue.

25) What is the difference between Promises and async/await?

=> Promises use .then() and .catch() for chaining, while async/await provides a cleaner, synchronous-like syntax for handling asynchronous code. Under the hood, async/await is just syntactic sugar over Promises.

26) How does JavaScript handle callback functions internally?

=> Callback functions are passed as arguments to asynchronous functions. When the async task completes, the callback is pushed into the task queue and executed when the call stack is empty.

 27) What is the difference between process.nextTick and setImmediate in Node.js?

=> process.nextTick: Executes callbacks immediately after the current operation, before I/O tasks.

setImmediate: Executes callbacks in the next iteration of the Event Loop, after I/O tasks.

28) What is the Job Queue in JavaScript, and how does it prioritize tasks?

=> The Job Queue is where Microtasks (like Promises) are stored. It has higher priority than the Callback Queue (where Macrotasks are stored). Microtasks always run before the next Macrotask.

29) How does requestAnimationFrame work in JavaScript?

=> requestAnimationFrame schedules a function to run before the next screen repaint (around 16ms for 60fps). It is used for smooth animations without blocking the main thread.

Modules, Concurrency, and Performance

30) What are JavaScript Modules, and how do they work?

=> JavaScript Modules allow code to be split into separate files and imported/exported using import and export keywords. This improves code organization and maintainability.

31) What is the difference between CommonJS and ES6 Modules?

=> CommonJS: Used in Node.js (require() and module.exports)

=> ES6 Modules: Used in modern JavaScript (import and export)
ES6 Modules support static analysis and tree shaking.

32) How does tree shaking work in JavaScript bundlers like Webpack?

=> Tree shaking removes unused code from the final bundle by analyzing module imports and eliminating dead code, reducing the bundle size and improving performance.

33) What are Web Workers, and how do they improve JavaScript performance?

=> Web Workers allow JavaScript to run in background threads, preventing the main thread from blocking. They are useful for CPU-intensive tasks like image processing.

34) What is the difference between synchronous and asynchronous JavaScript?

=> Synchronous: Executes one task at a time, blocking further execution.

Asynchronous: Allows multiple tasks to run concurrently using Callbacks, Promises, or async/await.

35) How does JavaScript handle multi-threading and concurrency?

=> JavaScript itself is single-threaded, but it can achieve concurrency using Web Workers, async operations, and event-driven programming.

36) What is requestIdleCallback, and how does it optimize performance?

=> requestIdleCallback schedules low-priority tasks when the browser is idle, preventing performance bottlenecks.

37) What is the difference between Debouncing and Throttling?

=> Debouncing: Delays execution until after a specified time has passed since the last function call.

Throttling: Limits the function execution to once per specified interval.

38) What is the difference between imperative and declarative programming in JavaScript?

=> Imperative: Focuses on how things should be done (e.g., for loops).

Declarative: Focuses on what should be done (e.g., .map(), .filter()).

39) How does JavaScript handle BigInt and floating-point precision?

=> BigInt: Used for handling large integers beyond Number.MAX_SAFE_INTEGER.

Floating-point precision: JavaScript numbers use IEEE 754, leading to precision issues in decimals (e.g., 0.1 + 0.2 !== 0.3). toFixed() and Math.round() help manage precision.

