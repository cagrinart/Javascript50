Lessons Learned From This Project 
==================================

## JavaScript
---

1. [**Array.prototype.some**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)

    Tests whether at least one element in the array passes the test implemented by the provided function. It returns a Boolean value.

    ```JavaScript
    const array = [1, 2, 3, 4, 5];
    // checks whether an element is even
    const even = (element) => element % 2 === 0;
    console.log(array.some(even));
    // expected output: true

    ```

2. [**Array.prototype.every**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every)

    Tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.


3. [**Array.prototype.slice**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)

    Returns a new array from start to end indexes. Original array will not modified.

    ```JavaScript
    const animals = ['ant', 'bison', 'camel', 'duck', 'elephant'];
    console.log(animals.slice(2));
    // expected output: Array ["camel", "duck", "elephant"]
    console.log(animals.slice(2, 4));
    // expected output: Array ["camel", "duck"]
    ```


4. [**... spread**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

    Expands an iterable or a string.

    ```JavaScript
    function sum(x, y, z) {
        return x + y + z;
    }
    const numbers = [1, 2, 3];
    console.log(sum(...numbers));
    // expected output: 6 
