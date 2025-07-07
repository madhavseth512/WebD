# CSS Properties

### CSS Colors
We can change background color or the text color. <br>
For Example- <br>
```CSS 
html{
    background-color = red;
    /*This changes the background of HTML document to red*/
}

h1{
    color = blue;
}
```
In CSS we have "named colors" which is a data type and acts as a keywords for the color code. Instead of using hexadecimal, RGB, or HSL values we can directly use these keywords to set the color of HTML elements. Syntactically, a named color is an "ident", a short form of identifier which is a sequence of characters that serves as a name for something.<br>

Here is the link to list of all the color codes with their named colors- <br>
[Named Colors](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)

But if we want to choose more variety of colors then we have a website called [Color Hunt](https://colorhunt.co/). It consists of hexcodes of different colors and we can use them instead of named colors. 
```CSS
h1{
    color: #0E2148;
}
```
<br>

**NOTE:** We can set both the text color and the background color for a text. This is done using the code:
```CSS
h1{
    color: blue;
    background-color: red;
}
```
And this will look something like - 
![Text and BG Color Example](../Images/text%20color%20and%20background%20color.png)


### CSS Font Properties
All basic fundamentals of text/font styling which includes font weight, family, size, color etc.<br>
```CSS
h1{
    color: blue;
    font-weight: bold;
    font-size: 10 px;
    font-family: sans-serif

    }
``` 
#### Font-Size 
Here we have 5 different methods:

- **Pixel or px** - This is an absolute unit for screen displays. 1px = 1/96th of an inch.
- **Point or pt** - This is also absolute unit. 1pt = 1/72nd of an inch.
- **em** - This font size unit is relative to the font-size of parent element(typically the width of a capital letter M contained inside parent element). If we set the font size of an element as 1 em then its font size will be exactly same as that of parent element, if set to 2em then it will be twice the parent size type.  
- **rem** - The rem unit is relative to the font-size of the  root element of the HTML document (usually the < html > tag )
- There are also set of **absolute-size keywords** that represent different font sizes. These are - xx-small, x-small, small, medium, large, x-large, xx-large, xxx-large. These keywords are mapped to specific sizes by the browser. The actual pixel size associated with each keyword can vary slightly between browsers. 

#### Font-Weight 
This sets how bold the text is. In case many font variables are avaiable then we have light, normal, bold, extrabold etc but we mostly use normal and bold.<br>
 - **normal , bold** - Normal and Bold font weight.
 - **lighter, bolder** - Sets the current element boldness to be one step lighter or heavier than parents element boldness. 
 - **100-900** - Numeric boldness values that provide finer grained control over above keywords. 

 #### Font-Family 
This allows us to specify a font for the browser to apply to the selected elements. The browser will only apply a font if it is avaiable on the machine the website is accessed on if not then it will use the browser default font. Web safe fonts are those which are without worry avaiable across all the systems, these are arial, Courier New, Georgia, Times New Roman, Trebuchet MS, Verdana. In case we specified a font and it is not avaiable on the system then we give the attribute of default fonts - serif, sans-serif, monospace, cursive, fantasy.<br>
Example - 
```CSS
p{
    font-family: Helvetica, Arial, sans-serif;

    /*HERE IF A FONT NAME HAS SPACES IN BETWEEN THEN IT SHOULD BE ENCLOSED IN DOUBLE QUOTES*/
     
    /*here browser will first try to use the "Helvetica" font if not installed then will try to use "Arial", if this not too then there is default font "sans-serif" */
}
```
**NOTE :** If we want to select a custom font from lets say google fonts then we should follow the process - select the font - get font button - get embbed code now copy the code and paste it in your source code with < head > tag of your HTML document. The link here is placed within head tag to correctly fetch the external resources like CSS files. The style tag also comes in the head tag.
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&family=Rubik:ital,wght@0,300..900;1,300..900&display=swap" rel="stylesheet">
</head>
<body>

</body>
</html>
```
#### Text-Align
This attribute is used for aligning the text. It contains of values like :<br>
- Center - Aligns text to center of the container
- Left - Aligns text to left of the container
- Right - Aligns text to the right of the continer
- Justify - Stretches the line so that each line has equal width. Extra spaces is distributed between the words. 
- Start - For left to write languages (eg English) this behaves like left. In right to left languages (eg Arabic) it behaves like right.
- End - This is just opposite of alignment of Start align. 

### Inspecting CSS
We can open developer tools by ctrl + shift + I. Here we get featues of elements tab, we get to visualize the box model of our website. In sources tab we get the original code from the website sources. Navigating and playing through it will help in getting familiar with the tool. 

### CSS Box Model - Margin, Padding and Border
