## How to use style in HTML
To add the style there are three main ways.  
* Use the inline style.
* Use the style tag in the head tag and write your styles there.  
* Use the external .css file and link that in your html.

## How to add custom fonts
There are many ways to add custom fonts but here I am using the google fonts to add the custom font.  
To add google font, go to there website and select the required font and get the link tag and add it in the HTML file, above the style.css .

## Basic Selectors
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
    color: red
}
```
Now all the elements that have class "blog-post" will get red text color.
