![index.html](screenshot/Clock.png)

Lessons Learned From This Project 
==================================

## HTML
---
1. [**class attribute**](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class) Defines space separated list of case sensetive classes. As in example below `hand` and `hour-hand` and separate classes.

    ```Html
    <div class="hand hour-hand"></div>
    ```
    
## CSS
---
1. [**box-shadow**](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) 
    
    Adds shadow effect around element
    
    _box- shadow: offset-x | offset-y | blur-radius | spread-radus | color_

    **_inset_** is optional and changes the outer shadow to inner shadow


## JavaScript and DOM
---

1. [**Dynamic Styling**](https://developer.mozilla.org/en-US/docs/Web/API/CSS_Object_Model/Using_dynamic_styling_information)

    Style of an element can be changed dynamically with CSS Object model(CSSOM)

    ```JavaScript
    const secondHand = document.querySelector('.second-hand');
    secondHand.style.transform = `rotate(45deg)`;
    ```
    Style of an element can also be changed alternatively using `setAttribute` method.

    ```JavaScript
    secondHand.setAttribute('style', 'transform: rotate(45deg);')`;
    ```

