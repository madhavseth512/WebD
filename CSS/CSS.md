# CSS (Cascading Style Sheets)
This is a Style Sheet language like HTML is a Markup Language. The SS is a computer language that defines the presentation or appearence of structured documents.<br>
There are other Style Sheet languages like Sass (Syntactically awesome style sheets) and Less (Leaner Style Sheets).<br>

### How to add CSS ?
There are three ways to add CSS to an HTML document.<br>

1. **Inline CSS** - Using this we apply CSS styles directly to an individual element using the 'style' attribute (It is a global attribute). This is quite cumbersome as there are plenty of elements and if we want them to share same styles then we have to add inline CSS to each and every one of them. 
```HTML
<p style = "color: blue fontsize: 16px">This paragraph tag contains text of blue color and 16 pixels font size.</p>

<html style = "background: blue">
</html>
```
2. **Internal/Embeded CSS** - Instead of placing style attribute within each element internal CSS uses style tags within the head tag. If our website has more than one webpages then it is better to use External CSS as we would have to repeat internal stylesheet across every webpage. Here the selector refers to the HTML element that we want to add styling element to. This selector basically acts as a filter or a search query that browser uses to find which HTML element we want to style. This selector basically can be HTML tag itself, classes, id attributes etc.  
```HTML
<!DOCTYPE HTML>
<html>
    <head>
        <style>
            /* CSS RULES GO HERE
            selector1 {
                property: value;
                background-color: yellow; 
            }

            selector2 {
                another_property: another_value;
                color: red;
            }
            */

        </style>
    </head>
    <body>CONTENTS OF THE BODY COME HERE</body>
</html>
```
3. External CSS - Better way to style larger website is to create seperate CSS file(s) with .css extension which contains all our CSS rules and then link them to the HTML documents. 

```HTML 
<!DOCTYPE html>
<html>
    <head>
        <link rel = "stylesheets"
              href = "FILE PATH TO PARTICULAR .css file"  
        />
    </head>
</html>

Here this link tag is a self closing tag. The rel attribute specifies the relationship between linked document and the current document. Here, it indicates the linked file is a stylesheet document.
Also the href attribute has the value of the file path of the related CSS code file.
```
### CSS Selectors
The CSS selector is the first part of the CSS rule that helps us choose which element we want to add CSS stying to. There are different ways in which we can select our elements. Some of these are: <br>

```HTML
<h2>Red</h2>
<h2>Green</h2>
<h2>Blue</h2>

We want to color every h2 heading according to the color named but we cannot select the CSS rule based on h2 heading thus we give different classes, ids and other specifications for selector to classify according to our need.
```

1. **Element Selector:** We classify according to different elements of the HTML 
```CSS
h2 {
    color: red;
}

/* This will convert all the h2 headings to red color*/  
```
2. **Class Selector:** These selects all HTML elements that have specified class attribute. Multiple HTML elements can have same class attribute. The value of the class just after dot in the style tag should be exactly same as that mentioned in the attributes i.e. it is case-sensitive.  
```HTML
<head>
    <style>
        /*Here the syntax starts with a dot and then name of the class*/
        .red-text{
            color: red;
        }
    </style>
</head>
<body>
    <h2 class = "red-text">Red</h2>
    <h2>Blue</h2>
    <h3>Green</h3>
</body>

This will convert our h2 heading text into red color. 
```
3. **ID Selector:** This selects the HTML element that has specified ID attribute for an HTML element. The difference between the ID selector and Class selector is that multiple HTML elements can have same class but multiple elements cannot have same id.

```HTML
<head>
    <style>
        #main{
            color: red
        }
    </style>
</head>
<body>
    <h2 id = "main">Red</h2>
    <h2 id = "id_2">Blue</h2>
    <h2>Green</h2>
</body>
```
4. **Attribute Selector:** These select elements based on the presence or value of their attributes.
```HTML
<p>
```
