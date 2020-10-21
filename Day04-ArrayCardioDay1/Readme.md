![index.html](screenshot/CssVariables.png)

Lessons Learned From This Project 
==================================

## HTML
---
1. [**Associating a label with an input**](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label) element has some advantages such as;
    * The label is programmatically associated with the input element
    * Clicking the label activates the input element

    The `<label>`'s `for` attribute and the `<input>`'s `id ` attribute needs to be same. 

    ```Html
    <label for="spacing">Spacing:</label>
    <input id="spacing" type="range" name="spacing" min="10" max="200" value="10" data-sizing="px">
    ```

    Alternatively, label can be associated with and input element bey nesting the input element. `id` attribute is not needed  for this implicit case asssociation.

    ```Html
    <label >Spacing:
        <input type="range" name="spacing" min="10" max="200" value="10" data-sizing="px">
    <label>
    ```

    
## CSS
---
1. [**Css variables**](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) 
    
    Declaring variables or custom properties begins with double hypen `--`
    ```Css
    :root {
        --spacing: 10px;
    }
    ```
    And can be used anywhere inside the `var()` function
    ```Css
    img {
        padding: var(--spacing);
    }
    ```
2. [**Filter**](https://developer.mozilla.org/en-US/docs/Web/CSS/filter) is a CSS property applies graphical effects to an element such as blur, color shift ,grayscale etc.
    ```Css
    img {
        filter: blur(var(--blur));
    }
    ```


## JavaScript and DOM
---

1. [**documentElement**](https://developer.mozilla.org/en-US/docs/Web/API/Document/documentElement)

    returns the Element that is the root element of the document (for example, the `<html>` element for HTML documents).

2. [**CSSStyleDeclaration.setProperty**](https://developer.mozilla.org/en-US/docs/Web/API/CSSStyleDeclaration/setProperty)

    This is a method interface sets a new value for a property on a CSS style declaration object.

    ```JavaScript
    style.setProperty(propertyName, value, priority);
    ```