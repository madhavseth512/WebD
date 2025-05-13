# HyperText Markup Language

### HTML HEADING ELEMENTS
There are 6 different HTML elements from h1 to h6. The h1 represents the most important heading on the page while h6 represents the least important. The idea comes from the heirarcy that we follow in a book. <br>
- Elements are different from Tags in HTML language. Element consists of opening tag, content within the tags and closing tag.<br>

```html
<h1>Content within opening and closing tag</h1>
<h2>Heading 2</h2>

```
<br>

Click on the link below to refer the documentation for HTML <br>
[HTML Documentation link](https://developer.mozilla.org/en-US/docs/Web/HTML)

### HTML PARAGRAPH ELEMENTS
Paragraphs are block level elements. These are usually represented in the visual media as blocks of text seperated from other blocks by a line or first level indentation but HTML paragraphs can be structural grouping of any elements be it forms or images etc etc. <br>

```HTML
<p>This is first paragraph of text</p>
<p>This will be second paragraph of text</p>
```
- There is a difference between line break tag and paragraph tag. Paragraph tag adds spacing before and after a paragraph as it is a block level tag. It requires a closing tag whereas line break tag is an inline tag, does not adds vertical spacing and continues the text from next line. Line break tag does not require a closing tag. 

### HTML VOID ELEMENTS
HTML void elements are those that do not have content in between them and thus they do not require closing tag.<br>

- Horizontal Rule Tag - This creates a horizontal ruling. Browsers displayed it as a horizontal ruling across the page.
- Line Break Tag - This tag is an inline tag. It is used for starting the upcoming text from a different line. Example if you are writing a poem then you will need this tag. 
```HTML
<hr/> - This is a horizontal rule tag
<br/> - This is a line break tag
Here we can omit / (forward slash) but its better not to do so because because it reminds that it is a self closing tag.
```
### HTML LISTS

1. **Unordered Lists :** These are used when order is not important in list items. These have attribute called "types" and their values are "square", "circle", "disc".<br>
2. **Ordered Lists :** These are used when order of the list is important. These have attributes like "reversed" which starts counting in decreasing order, another attribute called "start" in which we can give values like "5" (any number from which we wish to start counting) and also "type" which can have values like "A", "a", "i"(Roman numerals in lowecase),"I"(Roman numerials in uppercase),"1"(This is default)<br>


```HTML
UNORDERED LIST SYNTAX - 
<ul>
    <li>This is a list item of an unordered list.</li>
    <li>This is the second list item of unordered list.</li>
</ul>

ORDERED LIST SYNTAX - 
<ol>
    <li>First item of ordered list</li>
    <li>Seconf item of ordered list</li>
</ol>

EVERY LIST'S INDIVIDUAL ITEM IS DEFINED BY <li> and </li>. 
```

- NESTING AND INDENTATION - Nesting of a list is placing either ordered or unordered list inside a list item of another list. This creates a heirarchial structures within our list. HTML is indentation free in terms of its output it should be done for better readability. 
```HTML
<ol>
    <li>First element of my list</li>
    <li>Second element of my list</li>
    <li>Creating heirarcy within third element.
        <ul>
            <li>Bullet point 1</li>
            <li>Bullet point 2</li>
        </ul>
    </li>
    <li>Fourth element of my nested list</li>
</ol>
```

### ANCHOR ELEMENT
The anchor element in HTML is used to create hyperlink to other webpages, files, location within the same page, E-mail address or any other URL. This makes the web interconnected. The basic syntax of anchor element is opening anchor tag with attributes and their values specified, the text within the anchor tag and closing anchor tag.<br>
```HTML
<a href = https://www.google.com>Click to open Google</a>

We can provide many attributes seperated by space. Every attribute have attribute name = "value"
```

In addition to local attributes that an element have we have some global attributes that can be used for each and every tag in HTML. 
```HTML
<a href = https//:www.google.com draggable = true>Click to open Google</a>
This draggable attribute whould allow to drag the link anywhere on the screen.This uses drag and drop API.
```
When we are creating a list of hyperlinks then in syntax we have to incorporate the anchor tag within the individual list item tag in ordered or unordered list. <br>

### IMAGE ELEMENT
This is a void element and is thus a self closing tag. Through this we can add images in our webpages. The "src" attribute is required and it contains the path to the image you want to embed. The "alt" attribute is the textual representation of the image which is useful in accessibility (screen readers in case of visually imapred users) and also this text is displayed when the image is unable to load.
```HTML
<img src = "https://picsum.photos/200" alt = "Randomized Images"/>
There are two attributes here and after the link of the photo we provide the dimensions to the image in pixels. Here is only single nummber is added then it means we provided the width and it automatically adjusts the height according to aspect ratio of the image

<img src="https://picsum.photos/200/300" alt="Randomized 200x300 Image"/>
Here we have provided both width and height of the image.
```

### File Paths
A file path is a string of characters that specifies the unique location of a file or a directory within the file system. This tells system how to navigate through folders to find what you are looking for.<br>
**The Root Folder** is the topmost directory in the file's system heirarcy. In windows it is harddrive or C drive. <br>
Types of File Paths - <br>
- Absolute file path - It is the file path that starts from the root folder of the 