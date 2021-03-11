![index.html](screenshot/KeySequenceDetection.png)

Lessons Learned From This Project 
==================================

## JavaScript
---

1. [**Array.prototype.splice**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)

    Slice changes the content of an array by removing the items or replacing the element in place which are removed.
    
    ```
    let newArray = arr.splice(start, del_count, item1, item2..)
    ```
    start begins from 0 for the fist element and begins from -1 for the last element. del_count is omitted if the value is 0 or negative. items to add is optinal.

    ```JavaScript
    let myFish = ['angel', 'clown', 'drum', 'sturgeon']
    let removed = myFish.splice(2, 1, 'trumpet')

    // myFish is ["angel", "clown", "trumpet" ,"sturgeon"]
    // removed is ["drum"]
    ```

