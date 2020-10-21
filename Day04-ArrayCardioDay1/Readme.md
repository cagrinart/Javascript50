Lessons Learned From This Project 
==================================

## JavaScript
---

1. [**Array.prototype.filter**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

    The filter() method creates a new array with all elements that pass the test implemented by the provided function.

    ```JavaScript
    const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
    const result = words.filter(word => word.length > 6);
    console.log(result);
    // expected output: Array ["exuberant", "destruction", "present"]
    ```

2. [**Array.prototype.map**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)

    The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

    ```JavaScript
    const array1 = [1, 4, 9, 16];
    // pass a function to map
    const map1 = array1.map(x => x * 2);
    console.log(map1);
    // expected output: Array [2, 8, 18, 32]
    ```

3. [**Array.prototype.sort**](hhttps://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)

    The sort() method sorts the elements of an array in place and returns the sorted array.
    Built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values

    ```JavaScript
    const array1 = [1, 30, 4, 21, 100000];
    array1.sort();
    console.log(array1);
    // expected output: Array [1, 100000, 21, 30, 4]
    ```

    arr.sort([compareFunction])
    * If compareFunction(a, b) returns less than 0, sort a to an index lower than b (i.e. a comes first).
    * If compareFunction(a, b) returns greater than 0, sort b to an index lower than a (i.e. b comes first).
    * If compareFunction(a, b) returns 0, leave a and b unchanged.

4. [**Array.prototype.reduce**](hhttps://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)

    The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in single output value

    ```JavaScript
    const array1 = [1, 2, 3, 4];
    const reducer = (accumulator, currentValue) => accumulator + currentValue;
    // 5 + 1 + 2 + 3 + 4
    console.log(array1.reduce(reducer, 5));
    // expected output: 15
    ```Lessons Learned From This Project 
==================================

## JavaScript
---

1. [**Array.prototype.filter**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

    The filter() method creates a new array with all elements that pass the test implemented by the provided function.

    ```JavaScript
    const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
    const result = words.filter(word => word.length > 6);
    console.log(result);
    // expected output: Array ["exuberant", "destruction", "present"]
    ```

2. [**Array.prototype.map**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)

    The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

    ```JavaScript
    const array1 = [1, 4, 9, 16];
    // pass a function to map
    const map1 = array1.map(x => x * 2);
    console.log(map1);
    // expected output: Array [2, 8, 18, 32]
    ```

3. [**Array.prototype.sort**](hhttps://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)

    The sort() method sorts the elements of an array in place and returns the sorted array.
    Built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values

    ```JavaScript
    const array1 = [1, 30, 4, 21, 100000];
    array1.sort();
    console.log(array1);
    // expected output: Array [1, 100000, 21, 30, 4]
    ```

    arr.sort([compareFunction])
    * If compareFunction(a, b) returns less than 0, sort a to an index lower than b (i.e. a comes first).
    * If compareFunction(a, b) returns greater than 0, sort b to an index lower than a (i.e. b comes first).
    * If compareFunction(a, b) returns 0, leave a and b unchanged.

4. [**Array.prototype.reduce**](hhttps://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)

    The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in single output value

    ```JavaScript
    const array1 = [1, 2, 3, 4];
    const reducer = (accumulator, currentValue) => accumulator + currentValue;
    // 5 + 1 + 2 + 3 + 4
    console.log(array1.reduce(reducer, 5));
    // expected output: 15
    ```