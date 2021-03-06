## How to use style in HTML
To add the style there are three main ways.  
* Use the inline style.
* Use the style tag in the head tag and write your styles there.  
* Use the external .css file and link that in your html.

## How to add custom fonts
There are many ways to add custom fonts but here I am using the google fonts to add the custom font.  
To add google font, go to there website and select the required font and get the link tag and add it in the HTML file, above the style.css .

> # Basic Selectors
Selectors are used to add the style on a certain part of your HTML code.  
Given below are few types of selectors:  
* ### Elements Selector  
When we use HTML elements or HTML tags to select the part of our code, then those elements or tags are called element selector.  
Example:  
```css
h1 {
    color: red;
}
```  
This above code selects the h1 tag and apply the red color to all the text that are written within the h1 tag.  
* ### Class Selector  
Class Selector is used when we have to apply the same style to all the elements that have the same class.  
Class selectors can be used by adding . before the class-name in the css file.  
Example:  
```html
 <!-- This is the HTML code -->
<h1 class="blog-post"> Main Heading</h1>
<p>This is the paragraph</p>
<div class="blog-post">More information</div>
```
```css 
/* This is the css code */
.blog-post {
    color: red;
}
```
Now all the elements that have class "blog-post" will get red text color.
  
* ### Universal Selector
Universal selector is used to select all the elements and it is rarely used. * is used as universal selector.
```css
* {
    color: red;
}
```
* ### ID Selector
We also can use ID selector to select the HTML element, but as we know that ID is unique. so the style will be applied to a perticular element with that ID.  
And we use # sign before ID name to select an element with id.  
Example:  
```css
#first-post {
    color: red;
}
```
* ### Attribute Selector
We can select any HTML tag by the attributes they have. It can also be used to select many elements based on their attribute.  
To select elements based on the attribute we have to use [attribute-name] as selector.  
Example:  
```html
 <!-- This is the HTML code -->
<button disabled>Click Me!</button>
```
```css 
/* This is the css code */
[disabled] {
    color: red;
}
```


> # CSS Specificity
If you want the good understanding of CSS then you must understand the CSS Specificity.  
CSS selectors have certain rules on the basis of these rules, it is determined that which style should be applied to which selector.  
According to MDN, Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.  
Simply put, if two CSS selectors applied to the same element, the one with higher specificity is used.  
You can also understand this in a simple way that, different selectors have deferent priorities.  
### Specificity Hierarchy
* Inline Styles have higher specificity.
* ID selectors have lower specificity than Inline Styles.
* Classes, Attributes and Pseudo-classes have lower specificity than than the ID selectors.
* Elements and Pseudo-elements have even lower specificity than the classes.  
#### If two selectors have the same specificity then the selector that is declared last will take precedence.

> # Inheritance
Inheritance means that elements inherit some styles from the parent element.  
In CSS, inheritance controls what happens when no value is specified for a property on an element.  
CSS properties can be categorized in two types:
* Inherited properties, which by default are set to the computed value of the parent element
* Non-inherited properties, which by default are set to initial value of the property

> # Combinator
A CSS selector can contain more than one simple selector. Between the simple selectors, we can add a combinator.  

There are four type of combinators in CSS:  

* ### Decendant selector (space)
The descendant selector matches all elements that are descendants of a specified element.  

The following example selects all \<p> elements inside \<div> elements:   

```css
div p {
    color: red;
}
```
* ### Child selector (>)
The child selector selects all elements that are the children of a specified element.  

The following example selects all \<p> elements that are children of a \<div> element:
```css
div > p {
    color: red;
}
```
* ### Adjacent sibling selector (+)
The adjacent sibling selector is used to select an element that is directly after another specific element.

Sibling elements must have the same parent element, and "adjacent" means "immediately following".  

The following example selects the first \<p> element that are placed immediately after \<div> elements:
```css
div + p {
    color: red;
}
```
* ### General sibling selector (~)
The general sibling selector selects all elements that are siblings of a specified element.  

The following example selects all \<p> elements that are siblings of \<div> elements: 
```css
div ~ p {
    color: red;
}
```

> # Selectors, Properties and Values
This given table describes what are Selectors, Properties and Values.  

| Selector    | Properties     | Values  |
|------       |--------        | --------|
|div          |background-color| red     |
|.blog-post   |width           | 30%     |
|#main-title  |color           | #fafafa |
|[disableb]   |margin          | 10px    |
|*            |display         |block    |  

## Value Types
Values are tightly coupled with specific properties.  

| Pre-defined Options  | Colors     | Length, Sizes & numbers  | Functions |
|------       |--------        | --------| ------|
|display: block;|background: red;| height: 100px; |  background: url(...);  |
|overflow: auto;   |color: #fafafa;| width: 30%;| transform: scale(...); |
|  |color: #ccc;| order: 1; |
___


