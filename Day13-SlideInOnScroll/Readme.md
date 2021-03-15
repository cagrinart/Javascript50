Lessons Learned From This Project 
==================================

## JavaScript
---

1. [**HTMLElement.offsetTop**](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetTop)

    Read-only property returns the distance of the outer border of the current element relative to the inner border of the top of the offsetParent node.

    If the distance relative to viewport is needed **getBoundingClientRect** method can be used.

2. [**arguments**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)

    arguments is an Array-like object accessible inside functions that contains the values of the arguments passed to that function

    ```JavaScript
    function func1(a, b, c) {
        console.log(arguments[0]);
        // expected output: 1
    }

    func1(1, 2, 3);
    ```

3. [**Function.prototype.apply**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply)

    he apply() method calls a function with a given this value, and arguments provided as an array (or an array-like object).

4. [**setTimeout**](https://www.w3schools.com/jsref/met_win_settimeout.asp)

    The setTimeout() method calls a function or evaluates an expression after a specified number of milliseconds.

    Syntax
    > setTimeout(function, milliseconds, param1, param2, ...)

4. [**clearTimeout**](https://www.w3schools.com/jsref/met_win_cleartimeout.asp)

    Prevent the function set with the setTimeout() to execute.
    
