# 102 Lecture04 Class Notes:


## What is CSS ? 

**CSS** (Cascading Style Sheets) is a declarative language that controls how webpages look in the browser, The browser applies **CSS** style declarations to selected elements to display them properly. A style declaration contains the properties and their values, which determine how a webpage looks.

**CSS** is one of the three core Web technologies, along with HTML and JavaScript. **CSS** usually styles HTML elements, but can be also used with other markup languages like SVG or XML.

Three Ways to Insert CSS
There are three ways of inserting a style sheet:
* External CSS
* Internal CSS
* Inline CSS

### External CSS
With an external style sheet, you can change the look of an entire website by changing just one file!
Each HTML page must include a reference to the external style sheet file inside the <link> element, **inside the head** section.

**Example**: <link rel="stylesheet" href="style.css">


### Internal CSS
An internal style sheet may be used if one single HTML page has a unique style.
The internal style is defined inside the <style> element, inside the head section.

**Example**: 

<head>
      <style>
              p{color: red;}
      </style>
</head>         

### Inline CSS
An inline style may be used to apply a unique style for a single element.
To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

**Example**: <p style="color:red;">


#### Want To Know More ? 
[Visit our Resources website](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)