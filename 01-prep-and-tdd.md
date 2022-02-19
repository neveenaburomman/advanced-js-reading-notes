
**Event Loop**

JavaScript has a runtime model based on an event loop which has the job of checking both the stack and the task queue ,and when the stack is empty it takes the first thing in the queue and push it to the stack in order  to be excecuted .


**JS callback functions**

 A callback function is  when we pass a function as a parameter to another function. The main idea behind callback functions is to execute asynchronous JavaScript code, because the function will not run before a task is completed, but will run immediately after the task is completed. We can write the same callback function as an Anonymous Function or  as an Arrow Function.


**JS Promises**

 JS Promises can handle multiple asynchronous operations easily and give us  better error handling than callbacks and events because they had limited functionalities and created unmanageable code. 
also promisses have advatgaes like ,Better flow of control definition in asynchronous logic and Improves Code Readability
we have four stage for promises : fulfilled => the action when promise  succeeded , rejected => Action when promise failed ,=> pending: when promise not fulfilled or rejected yet , and settled=> Promise has fulfilled or rejected.

**JS Async/Await**
 
Async/Await is the extension of promises which makes our code Asynchronous , Async =>  allows us to write promises based code as if it was synchronous and it checks that we are not breaking the execution thread ,and It operates asynchronously via the event-loop .
Await function => is  waiting  for the promise. we can used it in the async block only. It makes the code wait until the promise returns a result. It only makes the async block wait.



**Test-Driven Development**
Test Driven Development is a software development in order to  test cases before developing the actual code, we have three phases : coding, testing (in the form of writing unit tests) and design (in the form of refactoring).
