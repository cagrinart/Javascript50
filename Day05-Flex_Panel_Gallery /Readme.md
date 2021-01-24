
![index.html](screenshot/FlexPanel.png)

Lessons Learned From This Project 
==================================

## HTML
---
--

    
## CSS
---
1. [**Css selectors**](https://www.w3schools.com/cssref/css_selectors.asp) 
    
    
   `.name1.name2` Selects all elements with both name1 and name2 set within its class attribute
   `.name1 .name2` Selects all elements with name2 that is a descendant of an element with name1
   `#firstname` Selects the element with id="firstname"
   `*` Selects all elements
   `p.intro` Selects all p elements with class="intro"
   `div, p`	Selects all div elements and all p elements
   `div > p` Selects all p elements where the parent is a div element
   `div p` Selects all p elements inside div elements
   `div + p` Selects the first p element that are placed immediately after div elements
   `p ~ ul`	Selects every ul element that are preceded by a p element
   
   Click the link at the header for more selectors

2. [**box-sizing**](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

    Defines how the width and height of an element are calculated: should they include padding and borders, or not

    `content-box` does not include padding, border and margin
    `border-box`includes padding and border but not the margin `width = border + padding + width of the content`

3. [**transition**](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

    Transitions allows you to change property values smoothly, over a given duration.
    `transition: transition-property duration timing-function delay`

4. [**background-size**](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)

    Sets the size of the element's background image.
    
    `contain` Scales the image as large as possible within its container without cropping or stretching the image.
    `cover` Scales the image as large as possible to fill the container, stretching the image if necessary.
    `auto` Scales the background image in the corresponding direction such that its intrinsic proportions are maintained.
    `<length>` Stretches the image in the corresponding dimension to the specified length. 
    `<percentage>` Stretches the image in the corresponding dimension to the specified percentage of the background positioning area.

5. [**background-position**](https://www.w3schools.com/cssref/pr_background-position.asp)
    
    Sets the starting position of a background image.

6. [**flex**](https://developer.mozilla.org/en-US/docs/Web/CSS/flex)
    
    Shorthand for the following CSS properties:

    * flex-grow
    * flex-shrink
    * flex-basis

## JavaScript and DOM
---

1. [**transitionevent propertyName**](https://www.w3schools.com/jsref/event_transition_propertyname.asp)

    The propertyName property returns the name of the CSS property associated with the transition, when a transitionevent occurs.


    ```JavaScript
    document.getElementById("myDIV").addEventListener("transitionend", myFunction);

    function myFunction(event) {
        this.innerHTML = "Property name is: " + event.propertyName;
    }
    ```

2. [**classList**](https://www.w3schools.com/jsref/prop_element_classlist.asp)

    This property is useful to add, remove and toggle CSS classes on an element.

    ```Javascript
    document.getElementById("myDIV").classList.add("mystyle");
    ```